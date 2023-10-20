<script setup>
import HeaderTemplete from "./layout/header/HeaderTemplete.vue";
</script>

<template>
  <div class="container-fluid">
    <header class="text-center">
      <HeaderTemplete />
    </header>

    <main class="row justify-content-center">
      <div class="col-md-6">
        <div class="main-content">
          <!-- Contenido principal de tu aplicación -->
        </div>
      </div>
    </main>
  </div>
</template>

<style scoped>
/* Estilos personalizados */
.container {
  width: 1600px;
  margin: 0 auto;
}
.main-content {
  background-color: #f5f5f5;
  padding: 20px;
}
</style>
