<template>
  <Navbar />
  <Hero />
  <Sobre />
  <Conhecimentos />
  <Projetos />
  <Contato />
</template>

<script setup>
import Navbar from './components/Navbar.vue'
import Hero from './components/Hero.vue'
import Sobre from './components/Sobre.vue'
import Conhecimentos from './components/Conhecimentos.vue'
import Projetos from './components/Projetos.vue'
import Contato from './components/Contato.vue'
</script>

<style>
html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  font-family: 'Poppins', sans-serif;
}
.fade-in {
  opacity: 0;
  transform: translateY(30px);
  animation: fadeInUp .8s forwards;
}

@keyframes fadeInUp {
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
@media (max-width: 768px) {
  section {
    padding: 60px 20px !important;
  }
}
</style>
