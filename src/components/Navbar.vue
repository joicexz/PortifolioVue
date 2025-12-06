<template>
  <nav :class="['navbar', { scrolled: isScrolled }]">
    <ul>
      <li><a href="#sobre">Sobre mim</a></li>
      <li><a href="#conhecimentos">Conhecimentos</a></li>
      <li><a href="#projetos">Projetos</a></li>
      <li><a href="#contato">Contato</a></li>
    </ul>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      isScrolled: false,
    };
  },
  mounted() {
    window.addEventListener("scroll", this.handleScroll);
  },
  beforeUnmount() {
    window.removeEventListener("scroll", this.handleScroll);
  },
  methods: {
    handleScroll() {
      const sobreSection = document.getElementById("sobre");

      if (!sobreSection) return;

      const sobreTop = sobreSection.offsetTop;

      this.isScrolled = window.scrollY >= sobreTop - 50;
    },
  },
};
</script>

<style scoped>
.navbar {
  position: fixed;
  width: 100%;
  top: 0;
  padding: 20px 40px;
  display: flex;
  justify-content: center;
  z-index: 99;
  background: transparent;
  transition: 0.3s;
  font-family: "Poppins", sans-serif;
}

.navbar a {
  color: white;
  font-weight: 600;
  font-size: 18px;
  transition: 0.3s;
}

.navbar.scrolled {
  background: rgba(255, 255, 255, 0.35);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border-bottom: 1px solid rgba(255, 255, 255, 0.4);
}

.navbar.scrolled a {
  color: #e90337;
}

.navbar.scrolled a:hover {
  color: #F5493D;
}

ul {
  display: flex;
  gap: 30px;
  list-style: none;
}

a {
  text-decoration: none;
}

@media (max-width: 600px) {
  .navbar {
    opacity: 0;
    pointer-events: none;
    transition: opacity .3s;
  }
}

</style>
