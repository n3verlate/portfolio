<script setup>
  import Header from './components/Header.vue';
  import Footer from './components/Footer.vue';
  import Hero from './components/Hero.vue';
  import Technos from './components/Technos.vue';
  import About from './components/About.vue';
  import Projects from './components/Projects.vue';
  import Career from './components/Career.vue';
</script>

<template>
  <div>
    <Header />
    <main id="home" class="container mx-auto">
      <Hero />
      <Technos />
      <About />
      <Projects />
      <Career />
    </main>
    <Footer />
  </div>
</template>
