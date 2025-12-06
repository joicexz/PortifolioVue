<script setup>
import { projetos } from '../data/projetos.js'
</script>

<template>
  <section id="projetos" class="container">
    <h2 class="titulo">Projetos</h2>

    <div class="grid">
      <div v-for="p in projetos" :key="p.id" class="card">
        <h3>{{ p.title }}</h3>
        <p>{{ p.description }}</p>

        <div class="tech">
          <span v-for="t in p.tech" :key="t">{{ t }}</span>
        </div>

        <div class="links">
          <a :href="p.repo" target="_blank">GitHub</a>
          <a v-if="p.demo" :href="p.demo" target="_blank">Demo</a>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.container {
  padding: 100px 50px;
  background: #fff5e9;
}

.titulo {
  text-align: center;
  margin-bottom: 40px;
  font-family: 'Poppins';
  font-size: 2.4rem;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 30px;
}

.card {
  background: white;
  padding: 30px;
  border-radius: 12px;
  box-shadow: 0 0 20px rgba(0,0,0,.1);
  transition: .3s;
}

.card:hover {
  transform: scale(1.02);
}

.tech span {
  display: inline-block;
  background: #ffdb9c;
  padding: 6px 12px;
  border-radius: 20px;
  margin: 5px;
  font-size: .8rem;
}

.links a {
  display: inline-block;
  margin-right: 12px;
  margin-top: 10px;
  color: #ff3b00;
  font-weight: 700;
}
</style>
