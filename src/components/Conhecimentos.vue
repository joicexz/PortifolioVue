<template>
  <section id="conhecimentos" class="conhecimentos">
    <h2>Conhecimentos</h2>

    <div class="grid">
      <div class="item">
        <i class="fa-brands fa-html5"></i>
        <span>HTML</span>
      </div>

      <div class="item">
        <i class="fa-brands fa-css3-alt"></i>
        <span>CSS</span>
      </div>

      <div class="item">
        <i class="fa-brands fa-square-js"></i>
        <span>JavaScript</span>
      </div>

      <div class="item">
        <i class="fa-brands fa-vuejs"></i>
        <span>Vue.js</span>
      </div>

      <div class="item">
        <i class="fa-brands fa-php"></i>
        <span>PHP</span>
      </div>

      <div class="item">
        <i class="fa-brands fa-react"></i>
        <span>React Native</span>
      </div>

      <div class="item">
        <i class="devicon-typescript-plain"></i>
        <span>TypeScript</span>
      </div>

      <div class="item">
        <i class="devicon-kotlin-plain"></i>
        <span>Kotlin </span>
      </div>

      <div class="item">
        <i class="fa-brands fa-figma"></i>
        <span>Figma </span>
      </div>

      <div class="item">
        <i class="fa-brands fa-github"></i>
        <span>Git/GitHub </span>
      </div>

      <div class="item">
        <i class="fa-solid fa-pen-ruler"></i>
        <span>UX/UI </span>
      </div>

      <div class="item">
        <i class="fa-solid fa-mobile-screen-button"></i>
        <span>Design Responsivo </span>
      </div>
    </div>
  </section>
</template>

<style scoped>
.conhecimentos {
  padding: 100px 60px;
  background: white;
  font-family: "Poppins", sans-serif;
}

h2 {
  text-align: center;
  font-size: 2.2rem;
  margin-bottom: 40px;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
  gap: 30px;
}

.item {
  background: #fff3d8;
  padding: 30px 20px;
  border-radius: 16px;
  text-align: center;
  transition: 0.3s;
  cursor: pointer;
}

.item:hover {
  transform: scale(1.07);
  background: #ffcb80;
}

i {
  font-size: 2.4rem;
  color: #ff5d00;
}

span {
  display: block;
  margin-top: 12px;
  font-weight: 700;
}

@media (max-width: 480px) {
  .grid {
    grid-template-columns: 1fr 1fr;
  }
}
</style>
