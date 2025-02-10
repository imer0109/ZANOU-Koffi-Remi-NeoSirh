<template>
     <section class="relative lg:py-24 py-16 bg-slate-50 dark:bg-slate-800" id="contact">
            <div class="container relative">
                <div class="grid grid-cols-1 pb-6 text-center">
                    <h3 class="font-semibold text-2xl leading-normal mb-4">Contactez-nous</h3>

                    <p class="text-slate-400 max-w-xl mx-auto">Vous avez des questions ou besoin d’assistance ? Notre équipe est à votre disposition pour vous accompagner et répondre à toutes vos demandes. N’hésitez pas à nous contacter, nous serons ravis de vous aider !</p>
                </div><!--end grid-->

                <div class="grid md:grid-cols-12 grid-cols-1 items-center gap-6">
                    <div class="lg:col-span-7 md:col-span-6">
                        <img src="../assets/images/contact.svg" alt="">
                    </div>

                    <div class="lg:col-span-5 md:col-span-6">
                        <div class="lg:ms-5">
                            <div class="bg-white dark:bg-slate-900 rounded-md shadow dark:shadow-gray-700 p-6">
                                <form>
                                    <div class="grid lg:grid-cols-12 grid-cols-1 gap-3">
                                        <div class="lg:col-span-6">
                                            <label for="name" class="font-semibold">Nom & Prénom :</label>
                                            <input name="name" id="name" type="text" class="mt-2 w-full py-2 px-3 h-10 bg-transparent dark:bg-slate-900 dark:text-slate-200 rounded outline-none border border-gray-100 dark:border-gray-800 focus:ring-0" placeholder="Nom et Prénom :">
                                        </div>
        
                                        <div class="lg:col-span-6">
                                            <label for="email" class="font-semibold">Email :</label>
                                            <input name="email" id="email" type="email" class="mt-2 w-full py-2 px-3 h-10 bg-transparent dark:bg-slate-900 dark:text-slate-200 rounded outline-none border border-gray-100 dark:border-gray-800 focus:ring-0" placeholder="Email :">
                                        </div>

                                        <div class="lg:col-span-12">
                                            <label for="phone" class="font-semibold">Téléphone :</label>
                                            <input name="phone" type="number" id="subject" class="mt-2 w-full py-2 px-3 h-10 bg-transparent dark:bg-slate-900 dark:text-slate-200 rounded outline-none border border-gray-100 dark:border-gray-800 focus:ring-0" placeholder="Téléphone :">
                                        </div>
                                        <div class="lg:col-span-12">
                                            <label for="subject" class="font-semibold">Sujet :</label>
                                            <input name="subject" id="subject" class="mt-2 w-full py-2 px-3 h-10 bg-transparent dark:bg-slate-900 dark:text-slate-200 rounded outline-none border border-gray-100 dark:border-gray-800 focus:ring-0" placeholder="Sujet :">
                                        </div>
    
                                        <div class="lg:col-span-12">
                                            <label for="comments" class="font-semibold">Message :</label>
                                            <textarea name="comments" id="comments" class="mt-2 w-full py-2 px-3 h-28 bg-transparent dark:bg-slate-900 dark:text-slate-200 rounded outline-none border border-gray-100 dark:border-gray-800 focus:ring-0" placeholder="Message :"></textarea>
                                        </div>
                                    </div>
                                    <button type="submit" id="submit" name="send" class="h-10 px-6 tracking-wide inline-flex items-center justify-center font-medium rounded-md bg-primary text-white mt-2">Envoyer</button>
                                </form>
                            </div>
                        </div>
                    </div>
                </div>
            </div><!--end container-->
        </section>
</template>