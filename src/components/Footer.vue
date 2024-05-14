<script setup>
    import phoneIcon from '../assets/svg/phone.svg';
    import linkedinIcon from '../assets/svg/linkedin.svg';
</script>
<template>
    <footer id="contact" class="flex flex-col">
        <div class="grid grid-cols-1 md:grid-cols-2">
            <div class="bg-slate-950 text-white p-6 lg:p-12">
                <span class="block text-2xl mb-2">Collaborons ensemble !</span>
                <p class="text-sm">Je suis disponible pour discuter de vive voix de votre projet ou du poste à pourvoir !</p>
            </div>
            <div class="grid grid-cols-2 md:grid-cols-1 gap-6 p-6 lg:p-12">
                <div class="flex items-center">
                    <picture>
                        <img :src="phoneIcon" alt="Phone icon" width="25" />
                    </picture>
                    <span class="ml-4"><a href="tel:0622020661">06.22.02.06.61</a></span>
                </div>
                <div class="flex items-center">
                    <picture>
                        <img :src="linkedinIcon" alt="Linkedin icon" width="25" />
                    </picture>
                    <span class="ml-4"><a href="https://www.linkedin.com/in/alexandredhont" target="_blank">Mon profil LinkedIn</a></span>
                </div>
            </div>
        </div>
    </footer>
</template>