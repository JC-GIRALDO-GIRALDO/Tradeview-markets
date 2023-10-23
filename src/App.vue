<script setup>
import FooterTemplete from "./layout/footer/FooterTemplete.vue";
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
    <footer>
      <FooterTemplete />
    </footer>
  </div>
</template>

<style scoped>
/* Estilos personalizados */
.main-container {
  width: 100%;
  margin: 0 auto;
  top: 0;
  left: 0;
  right: 0;
  z-index: 0;
  position: relative;
}
.content-main-primary {
  width: 100%;
  margin-top: 100px;
  height: auto;
  position: fixed;
  z-index: 1;
}
.text-center {
  background: linear-gradient(#181f29, #181f29, #181f29, #f1f1f200);
  color: #fff;
  padding: 10px 0;
  position: fixed;
  z-index: 2;
  top: 0;
  left: 0;
  right: 0;
}
.footer {
  width: 100%;
  display: flex;
  flex-direction: column;
  position: sticky;
  z-index: 1;
}
.footer section {
  margin-top: 20px;
}
</style>
