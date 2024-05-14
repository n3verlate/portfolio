<script setup>
    import Logo from './Logo.vue';
    import Navigation from './Navigation.vue';
    import imgUrl from '../assets/illustration.png'
</script>
<template>
    <div class="hero pt-[70px] relative flex flex-col-reverse items-center lg:block">
        <div class="my-8">
            <h1 class="relative text-center lg:text-left text-slate-950 text-[34px] leading-[45px] lg:text-[60px] lg:leading-[65px] xl:text-[80px] xl:leading-[85px] 2xl:text-[100px] font-bold 2xl:leading-[110px] lg:py-32 2xl:py-64 lg:pl-16 z-10">Développeur web <br /> Front-end</h1>
        </div>
        <picture class="lg:absolute lg:top-1/2 lg:-translate-y-1/2 lg:right-24 w-[200px] lg:w-[436px] 2xl:w-[600px]">
            <img :src="imgUrl" alt="Illustration">
        </picture>
    </div>
</template>