<script setup></script>

<template>
  <nav class="navbar">
    <ul class="navbar-list">
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

const navbar = ref(null);

// Agregar lógica adicional aquí si es necesario
</script>

<style scoped>
.navbar {
  color: #fff;
  padding: 10px 0;
}

.navbar-list {
  list-style: none;
  display: flex;
  margin: 0;
  padding: 0;
}

.navbar-item {
  margin: 0 10px;
}

.navbar-item a {
  text-decoration: none;
  color: #fff;
}

/* Agregar estilos adicionales según tus necesidades */
</style>
