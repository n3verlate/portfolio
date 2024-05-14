<script setup>
    import Logo from './Logo.vue';
    import Navigation from './Navigation.vue';
</script>
<template>
    <header class="fixed w-screen backdrop-blur-2xl bg-white/80 z-50 px-6 py-3 lg:py-8 f">
        <div class="container mx-auto flex justify-between items-center">
            <Logo />
            <Navigation />
        </div>
    </header>
</template>