<template>
    <section class="relative md:py-24 py-16" id="about">
            <div class="container relative">
                <div class="grid md:grid-cols-12 grid-cols-1 items-center gap-6">
                    <div class="md:col-span-6">
                        <div class="lg:me-8">
                            <div class="relative">
                                <img src="../assets/images/about.jpg" class="rounded-full shadow dark:shadow-gray-700" alt="">

                                <div class="absolute top-1/2 -translate-y-1/2 start-0 end-0 mx-auto size-56 flex justify-center items-center bg-white dark:bg-slate-900 rounded-full shadow dark:shadow-gray-700">
                                    <div class="text-center">
                                        <span class="text-teal-500 text-2xl font-semibold mb-0 flex items-center"><count-up :end-val="15" class="counter-value text-6xl font-semibold"></count-up>+</span>
                                        <span class="font-semibold block mt-0">Years <br> Experience</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="md:col-span-6">
                        <div class="lg:ms-8">
                            <h6 class="text-teal-500 text-sm font-semibold uppercase mb-2">Who Are We ?</h6>
                            <h3 class="font-semibold text-2xl leading-normal mb-4">We're a global stakeholder <br> relations and partnership <br> building consultancy.</h3>

                            <p class="text-slate-400 max-w-xl mb-6">Get instant helpful resources about anything on the go, easily implement secure money transfer solutions, boost your daily efficiency, connect to other app users and create your own Techwind network, and much more with just a few taps. commodo consequat. Duis aute irure.</p>

                            <a href="" class="h-10 px-6 tracking-wide inline-flex items-center justify-center font-medium rounded-md bg-teal-500 text-white">Read More <i class="mdi mdi-chevron-right align-middle ms-0.5"></i></a>
                        </div>
                    </div>
                </div>
            </div><!--end container-->
        </section>
</template>

<script setup >
    import CountUp from 'vue-countup-v3'
</script>