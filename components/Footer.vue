<template>
    <footer class="footer bg-dark-footer relative text-gray-200 dark:text-gray-200">
        <div class="py-[30px] px-0 border-t border-slate-800">
            <div class="container relative">
                <div class="grid lg:grid-cols-12 gap-6 items-center">
                    <div class="lg:col-span-6 md:text-start text-center">
                        <p class="mb-0">
                            Copyright © {{ date }} 
                            <NuxtLink to="https://neostart.tech/" target="_blank" class="text-[#0097b2] hover:underline">
                                Neo Start Technology
                            </NuxtLink>
                            Tous droits réservés.
                        </p>
                    </div>
                    <div class="lg:col-span-6 md:text-end text-center">
                        <p class="mb-0">
                            Contactez-nous : 
                            <NuxtLink to="mailto:contact@neosirh.com" class="text-[#0097b2] hover:underline">
                                contact@neosirh.com
                            </NuxtLink>
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
import feather from 'feather-icons'

export default {
    data() {
        return {
            date: new Date().getFullYear()
        }
    },
    mounted() {
        feather.replace();
    }
}
</script>
