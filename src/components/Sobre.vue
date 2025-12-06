<template>
  <section id="sobre" class="sobre fade-in">
    <h2>Sobre mim</h2>

    <div class="content">
      <img src="../assets/perfil.jpeg" alt="foto" class="foto" />

      <p>
        Olá, me chamo Joice Soares de Almeida, sou desenvolvedora Front-End
        apaixonada por criar interfaces intuitivas, bonitas e funcionais. Tenho
        experiência com HTML, CSS, JavaScript, PHP e React Native. Busco sempre
        estudar novas tecnologias e transformar ideias em projetos reais.
      </p>
    </div>
  </section>
</template>

<style scoped>
.sobre {
  padding: 100px 60px;
  background: #fffaf4;
  font-family: "Poppins", sans-serif;
}

h2 {
  font-size: 2.2rem;
  text-align: center;
  margin-bottom: 40px;
}

.content {
  display: flex;
  align-items: center;
  gap: 60px;
}

p {
  font-size: 1.2rem;
  line-height: 1.7;
  text-align: justify;
}

.foto {
  width: 220px;
  border-radius: 100%;
  box-shadow: 19px 14px 45px -9px rgba(224, 97, 72, 0.75);
  -webkit-box-shadow: 19px 14px 45px -9px rgba(224, 97, 72, 0.75);
  -moz-box-shadow: 19px 14px 45px -9px rgba(224, 97, 72, 0.75);
}

@media (max-width: 768px) {
  .content {
    flex-direction: column;
    text-align: center;
  }

  .foto {
    width: 160px;
  }
}
</style>
