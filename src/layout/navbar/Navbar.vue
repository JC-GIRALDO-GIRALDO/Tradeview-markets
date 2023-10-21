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
/* En tu estilo CSS para el menú */
.navbar {
  color: #fff;
  padding: 10px 0;
  text-align: center; /* Centra el texto horizontalmente */
}

.navbar-list {
  list-style: none;
  display: flex;
  justify-content: center; /* Centra los elementos del menú horizontalmente */
  margin: 0;
  padding: 0;
}

.navbar-item {
  margin: 0 20px; /* Aumenta el espacio entre los elementos del menú */
  margin-left: 50px;
  margin-right: 50px;
}

.navbar-item a {
  text-decoration: none;
  color: #fff;
}
/* Ajustes para pantallas pequeñas */
@media (max-width: 768px) {
  .navbar-list {
    flex-direction: column; /* Cambia a una disposición de columna en pantallas pequeñas */
    align-items: center; /* Centra los elementos verticalmente */
  }

  .navbar-item {
    margin: 10px 0; /* Espaciado entre los elementos del menú en pantallas pequeñas */
  }
}

/* Agregar estilos adicionales según tus necesidades */
</style>
