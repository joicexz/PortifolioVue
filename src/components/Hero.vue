<template>
  <section class="hero">
    <h1 class="title">Portfólio</h1>
    <h2 class="name">Joice Soares de Almeida</h2>
    <p class="desc">Desenvolvedora Front-End</p>
  </section>
</template>

<style scoped>
.hero {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
  color: white;
  background: linear-gradient(90deg, #e6004c, #ff3b00, #ff9d00);
  font-family: 'Poppins', sans-serif;
  position: relative;
}

.title {
  font-size: 7rem;
  font-family: 'Lobster Two', cursive;
  text-shadow: 0 0 20px rgba(255,255,255,.6);
}

.name {
  margin-top: 20px;
  font-size: 2rem;
  font-weight: 700;
}

.desc {
  font-style: italic;
  margin-top: 10px;
}
</style>
