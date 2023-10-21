<script setup>
import HeaderTemplete from "./layout/header/HeaderTemplete.vue";
</script>

<template>
  <div class="container-fluid"> <!-- Utiliza container-fluid en lugar de container -->
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
.container-fluid {
  width: 100%; /* Ancho completo para pantallas pequeñas */
  margin: 0 auto;
}

.main-content {
  background-color: #f5f5f5;
  padding: 20px;
}

/* Ajusta el padding para pantallas más pequeñas */
@media (max-width: 768px) {
  .main-content {
    padding: 10px;
  }
}
</style>
