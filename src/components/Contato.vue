<template>
  <section id="contato" class="contato fade-in">
    <h2>Vamos conversar?</h2>

    <p class="info">Entre em contato, responderei o mais breve possível!</p>

    <div class="contact-box">
      <a
        href="https://mail.google.com/mail/?view=cm&fs=1&to=joicesoaresalmeida@gmail.com"
        class="item"
      >
        <i class="fa-solid fa-envelope"></i>
        <span>joicesoaresalmeida@gmail.com</span>
      </a>

      <a href="tel:+5511917532483" class="item">
        <i class="fa-solid fa-phone"></i>
        <span>(11) 91753-2483</span>
      </a>
    </div>

    <div class="social">
      <a href="https://github.com/joicexz" target="_blank">
        <i class="fa-brands fa-github"></i>
      </a>

      <a href="https://instagram.com/joicexz._" target="_blank">
        <i class="fa-brands fa-instagram"></i>
      </a>
    </div>
  </section>
</template>

<style scoped>
.contato {
  padding: 100px 60px;
  background: #fffaf4;
  text-align: center;
  font-family: "Poppins";
}

h2 {
  font-size: 2.6rem;
  margin-bottom: 20px;
  color: #ff5b00;
}

.info {
  font-size: 1.1rem;
  margin-bottom: 40px;
  color: #333;
  opacity: 0.75;
}

.contact-box {
  display: flex;
  flex-direction: column;
  gap: 20px;
  max-width: 400px;
  margin: auto;
}

.item {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 12px;

  padding: 14px 20px;
  border-radius: 12px;
  background: #fff;
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.08);

  font-weight: 600;
  color: #333;
  text-decoration: none;
  transition: 0.3s;
}

.item i {
  font-size: 1.8rem;
  color: #ff5b00;
}

.item:hover {
  transform: translateY(-4px);
  box-shadow: 0 0 30px rgba(0, 0, 0, 0.12);
}

.social {
  margin-top: 50px;
}

.social i {
  font-size: 2.4rem;
  margin: 0 20px;
  color: #ff5b00;
  transition: 0.3s;
}

.social i:hover {
  transform: scale(1.2) rotate(3deg);
}

@media (max-width: 480px) {
  .contato {
    padding: 70px 20px;
  }

  .item {
    font-size: 0.95rem;
    padding: 12px 15px;
  }

  .social i {
    margin: 0 12px;
  }
}
</style>
