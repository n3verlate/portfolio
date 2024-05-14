<script setup>
    import vueLogo from '../assets/vuejs.png'
    import angularLogo from '../assets/angular.png'
    import magentoLogo from '../assets/magento.png'
</script>
<template>
    <div class="relative technos flex flex-col items-center text-white lg:mt-16 py-6 lg:py-12 bg-slate-950 before:bg-slate-950 after:bg-slate-950">
        <div class="flex gap-8">
            <picture class="w-[85px] lg:w-[140px] flex items-center">
                <img :src="vueLogo" alt="Vuejs logo">
            </picture>
            <picture class="w-[85px] lg:w-[140px] flex items-center">
                <img :src="angularLogo" alt="Angular logo">
            </picture>
            <picture class="w-[85px] lg:w-[140px] flex items-center">
                <img :src="magentoLogo" alt="Magento logo">
            </picture>
        </div>
    </div>
</template>
<style scoped>
    .technos::before, .technos::after {
        @apply absolute h-full top-0;
        content: '';
        width: calc((100vw - 100%) / 2);
        left: calc((100vw - 100%) / 2 * -1);
    }

    .technos::after {
        left: auto;
        right: calc((100vw - 100%) / 2 * -1);
    }
</style>