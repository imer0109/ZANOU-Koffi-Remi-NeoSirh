<template>
  <section class="relative md:py-24 py-16" id="whyNeoSirh">
    <div class="container relative">
      <div class="grid grid-cols-1 pb-6 text-center">
        <h3 class="font-semibold text-2xl leading-normal mb-4">
          Pourquoi choisir <span class="text-primary">NEO SIRH ?</span>
        </h3>

        <p class="text-slate-400 max-w-xl mx-auto">
          Une solution intelligente et complète pour automatiser, centraliser et
          optimiser la gestion des ressources humaines.
        </p>
      </div>

      <div class="grid md:grid-cols-12 grid-cols-1 mt-6 gap-6">
        <!-- left content -->
        <div class="lg:col-span-4 md:col-span-5">
          <div class="sticky top-20">
            <ul class="flex flex-col p-6 bg-white dark:bg-slate-900 shadow dark:shadow-gray-700 rounded-md">
              <li v-for="(item, index) in title" :key="index" role="presentation">
                <button class="px-4 py-2 text-start text-base font-medium rounded-md w-full duration-500 mt-6" :class="activeIndex === index
                  ? 'text-white bg-teal-500'
                  : 'hover:text-teal-500 dark:hover:text-white hover:bg-slate-50 dark:hover:bg-slate-800'"
                  @click="tabChange(index)" :aria-selected="activeIndex === index" role="tab">
                  <span class="text-lg mt-2 block">{{ item }}</span>
                  <span class="block mt-2 text-sm">
                    {{ description[index] }}
                  </span>
                </button>
              </li>
            </ul>
          </div>
        </div>

        <!-- right content -->
        <div class="lg:col-span-8 md:col-span-7">
          <div class="p-6 bg-white dark:bg-slate-900 shadow dark:shadow-gray-700 rounded-md">
            <div v-for="(item, index) in title" :key="index" v-show="activeIndex === index" role="tabpanel">
              <img :src="images[index]" class="shadow dark:shadow-gray-700 rounded-md w-full"
                :alt="`Illustration pour ${item}`" />
              <div class="mt-6">
                <h5 class="text-lg font-medium text-gray-800">{{ item }}</h5>
                <div class="text-gray-500 mt-4 flex flex-col gap-3">
                  <div v-for="(line, idx) in details[index].split('. ')" :key="idx" class="flex items-start gap-2 text-justify">
                    <div class="w-5 h-5 flex items-center justify-center rounded-full bg-[#0097b2] text-white">
                      <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2"
                        stroke="currentColor" class="w-5 h-5">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" />
                      </svg>
                    </div>
                    <span>{{ line }}</span>
                  </div>
                </div>
              </div>

            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";

const activeIndex = ref(0);

const title = ref([
  "Économie",
  "Fonctionnalité & Sécurité",
  "Gestion",
  "Opération",
  "Performance",
  "Expérience utilisateur",
]);

const description = ref([
  "Réduction des processus manuels pour un gain de temps et une meilleure productivité",
  "Toutes les informations RH accessibles en un seul endroit, en toute sécurité.",
  "Gestion fluide des demandes avec validation simplifiée pour les managers.",
  "Calcul automatisé des salaires et suivi des paiements sans erreurs.",
  "Outils intégrés pour mesurer et améliorer les performances des employés.",
  "Interface moderne et facile à utiliser pour les employés et les gestionnaires.",
]);

const images = ref([
  "/images/01.jpg",
  "/images/02.jpg",
  "/images/03.jpg",
  "/images/1.jpg",
  "/images/2.jpg",
  "/images/ab7.jpg",
]);

const details = ref([
  "Automatisation et simplification des tâches administratives afin de réduire la charge de travail manuel. Permettant ainsi aux équipes de se concentrer sur des missions à plus forte valeur ajoutée. Cette optimisation des processus améliore l’efficacité opérationnelle, réduit les risques d’erreur et favorise une gestion des ressources humaines plus fluide et réactive. Contribuant ainsi à un gain de temps précieux et à une augmentation globale de la productivité.",
  "Centralisation de l’ensemble des données et documents relatifs aux ressources humaines sur une plateforme unique, garantissant un accès rapide, structuré et sécurisé. Cette approche permet de simplifier la gestion RH, d’assurer une meilleure traçabilité des informations. Renforcer la confidentialité des données, tout en facilitant la prise de décision et la collaboration entre les équipes.",
  "Optimisation du traitement des demandes grâce à un système de gestion intuitif, permettant aux managers de valider facilement et rapidement les requêtes. Cette approche fluidifie les processus internes, réduit les délais de réponse et améliore l’expérience des collaborateurs en garantissant une gestion plus efficace et transparente.",
  "Automatisation du calcul des salaires et du suivi des paiements afin de garantir une gestion précise, rapide et sans erreur. Cette approche permet de réduire la charge administrative, d’assurer la conformité avec les réglementations. Permet de mettre en vigueur et d’offrir aux employés une transparence totale sur leur rémunération, tout en optimisant le processus de paie pour les services RH.",
  "Mise à disposition d’outils intégrés permettant d’évaluer, suivre et analyser les performances des employés de manière objective et efficace. Ces solutions favorisent une gestion proactive des talents, facilitent l’identification des axes d’amélioration. Contribuent à la mise en place de stratégies adaptées pour renforcer l’engagement et la productivité des équipes.",
  "Une interface intuitive, ergonomique et moderne conçue pour offrir une expérience utilisateur fluide aussi bien aux employés qu'aux gestionnaires. Grâce à une navigation simplifiée et des fonctionnalités accessibles, chacun peut facilement effectuer ses tâches. Consulter les informations essentielles et interagir avec les outils RH en toute simplicité, favorisant ainsi une adoption rapide et une meilleure efficacité au quotidien.",
]);

const tabChange = (index) => {
  activeIndex.value = index;
};
</script>
