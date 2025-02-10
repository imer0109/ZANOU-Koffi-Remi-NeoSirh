<template>
    <section class="bg-[#F5F7FA] py-10 px-6 md:px-16 " id="about">
        <div class="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-2 gap-8">
            <div class="flex flex-col gap-4">
                <div class="relative rounded-lg overflow-hidden">
                    <img src="../assets/images/qns.png" alt="Person working with tablet"
                        class="w-full h-auto object-cover" />
                </div>
            </div>

            <div class="text-left">
                <h2 class="text-2xl md:text-2xl font-bold text-gray-800 mb-4">Qui sommes-nous?</h2>
                <p class="text-gray-600 leading-relaxed mb-6 text-justify">
                    Nous sommes NEO START TECHNOLOGY, une entreprise togolaise spécialisée dans l’ingénierie
                    informatique et le développement de solutions technologiques innovantes. Fondée avec la
                    vision de révolutionner le secteur numérique en Afrique, notre mission est d’accompagner
                    les entreprises et organisations dans leur transformation digitale grâce à des solutions
                    performantes, sécurisées et adaptées à leurs besoins spécifiques. Notre expertise couvre
                    un large éventail de domaines, notamment :
                </p>

                <ul class="grid grid-cols-1 md:grid-cols-2 gap-4 mb-8">
                    <li class="flex items-center gap-2 text-gray-700">
                        <div class="w-5 h-5 flex items-center justify-center rounded-full bg-[#0097b2] text-white">
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2"
                                stroke="currentColor" class="w-5 h-5">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" />
                            </svg>
                        </div>
                        Développement de logiciels et d’applications web & mobiles
                    </li>
                    <li class="flex items-center gap-2 text-gray-700">
                        <div class="w-5 h-5 flex items-center justify-center rounded-full bg-[#0097b2] text-white">
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2"
                                stroke="currentColor" class="w-5 h-5">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" />
                            </svg>
                        </div>
                        Cybersécurité et protection des données
                    </li>
                    <li class="flex items-center gap-2 text-gray-700">
                        <div class="w-5 h-5 flex items-center justify-center rounded-full bg-[#0097b2] text-white">
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2"
                                stroke="currentColor" class="w-5 h-5">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" />
                            </svg>
                        </div>
                        Intelligence artificielle et big data
                    </li>
                    <li class="flex items-center gap-2 text-gray-700">
                        <div class="w-5 h-5 flex items-center justify-center rounded-full bg-[#0097b2] text-white">
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2"
                                stroke="currentColor" class="w-5 h-5">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" />
                            </svg>
                        </div>
                        Maintenance informatique
                    </li>
                    <li class="flex items-center gap-2 text-gray-700">
                        <div class="w-5 h-5 flex items-center justify-center rounded-full bg-[#0097b2] text-white">
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2"
                                stroke="currentColor" class="w-5 h-5">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" />
                            </svg>
                        </div>
                        Solutions cloud et infrastructures IT
                    </li>
                    <li class="flex items-center gap-2 text-gray-700">
                        <div class="w-5 h-5 flex items-center justify-center rounded-full bg-[#0097b2] text-white">
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2"
                                stroke="currentColor" class="w-5 h-5">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" />
                            </svg>
                        </div>
                        Conseil et audit en transformation numérique
                    </li>
                    <li class="flex items-center gap-2 text-gray-700">
                        <div class="w-5 h-5 flex items-center justify-center rounded-full bg-[#0097b2] text-white">
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2"
                                stroke="currentColor" class="w-5 h-5">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" />
                            </svg>
                        </div>
                        Communication et marketing numérique
                    </li>
                    <li class="flex items-center gap-2 text-gray-700">
                        <div class="w-5 h-5 flex items-center justify-center rounded-full bg-[#0097b2] text-white">
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2"
                                stroke="currentColor" class="w-5 h-5">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" />
                            </svg>
                        </div>
                        Vente de matériels informatiques et infogérance
                    </li>
                </ul>

                <div class="flex gap-6 items-center">
                    <a href="mailto:contact@neostart.com" target="_blank"
                        class="bg-[#0097b2] text-white font-semibold py-2 px-6 rounded-md shadow hover:bg-[#007a8f]">
                        Nous contacter
                    </a>
                    <a href="https://neostart.tech" target="_blank"
                        class="bg-white border border-gray-300 text-gray-800 font-semibold py-2 px-6 rounded-md shadow hover:bg-gray-100">
                        Voir plus
                    </a>
                </div>
                <div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped></style>