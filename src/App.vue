<script setup>
import HeaderTemplete from "./layout/header/HeaderTemplete.vue";
import MainTemplete from "./layout/main-contenido/MainTemplete.vue";
</script>

<template>
  <div class="container-fluid">
    <header class="text-center">
      <HeaderTemplete />
    </header>

    <main class="row justify-content-center">
      <div class="col">
        <div class="main-content">
          <MainTemplete />
        </div>
      </div>
    </main>
  </div>
</template>

<style scoped>
/* Estilos personalizados */
.container-fluid {
  width: 100%; /* Ancho completo para pantallas pequeñas */
  margin: 0 auto;
}

.main-content {
  background-color: #f5f5f5;
  width: 100%;
}
.col {
  width: 100%;
}
/* Ajusta el padding para pantallas más pequeñas */
@media (max-width: 768px) {
  .main-content {
    padding: 10px;
  }
}
</style>

