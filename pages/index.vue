<template>
  <div>
    <Navbar />
    <section class="relative overflow-hidden md:py-48 py-40 bg-secondary" id="home">
      <div class="container relative mt-8">
        <div class="grid md:grid-cols-2 grid-cols-1 gap-6 items-center">
          <div>
            <h3 class="font-semibold lg:leading-normal leading-normal tracking-wide text-4xl lg:text-4xl mb-5">Optimiser
              la gestion de vos ressources humaines avec <span class="text-[#0097b2]">NEO SIRH</span> </h3>
            <p class="text-slate-400 text-lg max-w-xl">Un système sur mesure pour la gestion de vos ressources humaines
            </p>

            <div class="mt-14">
              <ul class="flex items-center space-x-4">

                <!-- Bouton Démo -->
                <li class="nav-item contact">
                  <a href="https://demo.neosirh.com" target="_blank"
                    class="h-[45px] px-[35px] py-4 bg-[#0097b2] rounded-[20px] flex items-center gap-2">
                    <img src="../assets/images/demo.png" alt="Icône Démo" class="w-4 h-4">
                    <span class="text-white text-base font-semibold leading-normal">Démo</span>
                  </a>
                </li>

                <!-- Bouton Voir Documentation -->
                <li>
                  <a href="https://docs.neosirh.com" target="_blank"
                    class="w-[200px] h-[45px] px-4 py-4 bg-[#dff5f9] rounded-[20px] border border-[#0097b2] flex items-center justify-center">
                    <span class="text-[#0097b2] text-base font-semibold leading-normal">Voir documentation</span>
                  </a>
                </li>

              </ul>
            </div>

          </div>

          <div class="lg:ms-8">
            <div class="relative">
              <img src="../assets/images/head1.png" class="relative top-11" alt="">
              <!-- <div
                  class="overflow-hidden absolute md:size-[500px] size-[400px] bg-gradient-to-tl to-teal-500/20 via-teal-500/70 from-teal-500 bottom-1/2 translate-y-1/2 md:start-0 start-1/2 ltr:md:translate-x-0 ltr:-translate-x-1/2 rtl:md:translate-x-0 rtl:translate-x-1/2 -z-1 shadow-md shadow-teal-500/10 rounded-full">
                </div> -->
            </div>
          </div>
        </div>
      </div>
    </section>
    <Service />
    <PourquoiSIRH />
    <QuiSommeNous />
    <!-- <ContactUs/> -->
  </div>
</template>

<script>
import Navbar from "../components/Navbar.vue";
import About from "../components/About.vue";
import Features from '../components/Features.vue';
import AgencyTab from '../components/AgencyTab.vue';
import Cta from '../components/Cta.vue';
import Client from '../components/Client.vue';
import Pricing from '../components/Pricing.vue';
import Blogs from '../components/Blogs.vue';
import GetInTouch from '../components/GetInTouch.vue';
import PourquoiSIRH from "~/components/PourquoiSIRH.vue";
import ContactUs from "~/components/contactUs.vue";
import QuiSommeNous from "~/components/QuiSommeNous.vue";
import Loading from "~/components/Loading.vue";
export default {
  name: "IndexPage",
  data() {
    return {

    }
  },
  components: {
    Navbar,
    About,
    Features,
    AgencyTab,
    Cta,
    Client,
    Pricing,
    Blogs,
    GetInTouch,
  }

}
</script>

<style lang="scss" scoped></style>