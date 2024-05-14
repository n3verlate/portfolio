<script setup>
  import navIcon from '../assets/svg/bars.svg';
  import closeIcon from '../assets/svg/close.svg';
  import githubIcon from '../assets/svg/github.svg';
  import linkedinIcon from '../assets/svg/linkedin.svg';
  import { ref } from 'vue';

  const showNavigation = ref(false);

  function goTo(anchor) {

  }
</script>
<template>
  <div class="lg:flex gap-12 z-20" :class="{ 'flex fixed top-0 left-0 w-full h-screen bg-[#FB9828] flex-col items-center justify-center text-2xl': showNavigation, 'hidden': !showNavigation  }">
    <nav class="flex flex-col lg:flex-row items-center gap-12">
      <li>
        <a href="#home" @click="showNavigation = false">Accueil</a>
      </li>
      <li>
        <a href="#projects" @click="showNavigation = false">Mes projets</a>
      </li>
      <li>
        <a href="#career" @click="showNavigation = false">Mon parcours pro</a>
      </li>
      <li>
        <a href="#contact" @click="showNavigation = false">Me contacter</a>
      </li>
    </nav>
    <div class="flex gap-6">
      <!-- Logo Github -->
      <a href="https://github.com/n3verlate" target="_blank">
        <picture>
          <img width="32" :src="githubIcon" alt="Github icon">
        </picture>
      </a>

      <!-- Logo LinkdedIn -->
      <a href="https://www.linkedin.com/in/alexandredhont" target="_blank">
        <picture>
          <img width="32" :src="linkedinIcon" alt="Linkedin icon">
        </picture>
      </a>
	  </div>
  </div>
  <!-- Burger icon -->
  <picture v-if="!showNavigation" @click="showNavigation = true" class="lg:hidden cursor-pointer z-50">
    <img width="35" :src="navIcon" alt="Nav icon">
  </picture>
  <!-- Close icon -->
  <picture v-if="showNavigation" @click="showNavigation = false" class="lg:hidden cursor-pointer z-50">
    <img width="35" :src="closeIcon" alt="Close icon">
  </picture>
</template>
<style scoped>
  li {
    list-style: none;
  }
</style>
