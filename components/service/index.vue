<template>
  <section id="services">
    <div class="relative">
      <div
        class="absolute opacity-5 inset-0 bg-[url('assets/images/bg-service.png')] bg-cover"
      ></div>

      <div class="relative z-10 text-center p-5">
        <h1 class="text-2xl font-bold mt-10 mb-10">Nos missions</h1>
        <p class="">
          Offrir une solution centralisée et automatisée pour une administration
          <br />
          plus fluide, efficace et transparente
        </p>

        <div class="lg:flex justify-center lg:space-x-20 mt-10">
          <ServiceCard
            :image="img1"
            title="Automatisation"
            subTitle="Nous réduisons les tâches administratives répétitives pour que vous puissiez vous concentrer sur l’essentiel : vos collaborateurs"
          />
          <ServiceCard
            :image="img2"
            title="Transparence"
            subTitle="Chaque employé a accès à ses informations en toute sécurité, et les gestionnaires disposent d’outils clairs pour prendre de meilleures décisions."
          />
          <ServiceCard
            :image="img3"
            title="Performance"
            subTitle="Grâce à notre SIRH, suivez facilement les performances, gérez les évaluations et améliorez la productivité de votre entreprise."
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import img1 from "assets/images/mission1.png";
import img2 from "assets/images/mission2.png";
import img3 from "assets/images/mission3.png";

const services = ref([
  {
    id: 1,
    src: "assets/images/mission1.png",
    alt: "Image 1",
    title: "Automatisation",
    subTitle:
      "This is required when, for example, the final text is not yet available.",
  },
]);
</script>