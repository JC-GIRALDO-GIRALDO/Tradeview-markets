<script setup>
import HeaderTemplete from "./layout/header/HeaderTemplete.vue";
import MainTemplete from "./layout/main-contenido/MainTemplete.vue";
import Navbar from "./layout/navbar/Navbar.vue";
</script>

<template>
  <div class="main-container">
    <header class="text-center">
      <HeaderTemplete />
      <nav>
        <Navbar />
      </nav>
    </header>
    <main class="content-main-primary">
      <MainTemplete />
    </main>
    <footer></footer>
  </div>
</template>

<style scoped>
/* Estilos personalizados */
.main-container {
  width: 100%;
  margin: 0 auto;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1; /* Agrega una capa superior para mantener el encabezado visible */
}

.content-main-primary {
  width: 100%;
  margin-top: 100px; /* Ajusta el margen superior para separar el contenido del encabezado */
  height: auto;
}

.text-center {
  background: linear-gradient(#181f29, #181f29, #181f29, #f1f1f200);
  color: #fff;
  padding: 10px 0;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 2; /* Asegura que el encabezado esté por encima del contenido */
}

/* ... otros estilos ... */
</style>
