<template>
  <nav class="navbar">
    <!-- Botón de menú para pantallas pequeñas -->
    <button class="menu-button" @click="toggleMenu">☰</button>
    <ul class="navbar-list" :class="{ open: isMenuOpen }">
      <li class="navbar-item"><a href="#">Markets</a></li>
      <li class="navbar-item"><a href="#">Company</a></li>
      <li class="navbar-item"><a href="#">Accounts</a></li>
      <li class="navbar-item"><a href="#">Platforms</a></li>
      <li class="navbar-item"><a href="#">Pricing</a></li>
      <li class="navbar-item"><a href="#">Introducing Brokers</a></li>
      <li class="navbar-item"><a href="#">Education</a></li>
      <li class="navbar-item"><a href="#">Support</a></li>
    </ul>
  </nav>
</template>

<script setup>
import { ref } from "vue";

const isMenuOpen = ref(false);

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
};
</script>

<style scoped>
/* Estilo para el botón de menú en pantallas pequeñas */
.menu-button {
  font-size: 20px;
  cursor: pointer;
  display: none; /* Ocultar el botón por defecto */
  color: #f1f1f2;
  text-decoration: none;
}
.navbar-list {
  list-style: none;
  color: #f1f1f2;
  text-decoration: none;
}
.navbar-item a {
  color: #f1f1f2;
  text-decoration: none;
  margin-left: 40px;
  margin-right: 40px;
}
/* Ajustes para pantallas pequeñas */
@media (max-width: 768px) {
  .menu-button {
    display: block; /* Mostrar el botón en pantallas pequeñas */
  }

  /* Ocultar el menú por defecto en pantallas pequeñas */
  .navbar-list {
    display: none;
  }

  /* Mostrar el menú cuando isMenuOpen es verdadero en pantallas pequeñas */
  .navbar-list.open {
    display: block;
  }
}

/* Estilo CSS para el menú en pantallas más grandes */
@media (min-width: 769px) {
  .navbar-list {
    display: flex;
  }
}
</style>
