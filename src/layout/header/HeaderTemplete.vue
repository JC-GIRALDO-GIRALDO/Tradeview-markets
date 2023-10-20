<script setup>
import Forex from "../../components/Forex.vue";
import Futures from "../../components/Futures.vue";
import Stocks from "../../components/Stocks.vue";
import Tradegatehub from "../../components/Tradegatehub.vue";
import Login from "../../views/Login.vue";
import Contacto from "../../views/Contacto.vue";
import Language from "../../views/Language.vue";
</script>
<template>
  <header class="header-container">
    <div class="container">
      <div
        class="d-flex flex-column flex-md-row align-items-center justify-content-between"
      >
        <!-- Primera sección - Imagen -->
        <div class="section text-center mb-3 mb-md-0">
          <img
            src="../../../public/tvm-logo-black.png"
            alt="logo-tvm"
            class="logo"
          />
        </div>
        <!-- Segunda sección - Lista con clase personalizada -->
        <div class="section horizontal-list text-center mb-3 mb-md-0">
          <ul class="nav navigation-menu">
            <li class="nav-item"><Forex /></li>
            <li class="nav-item"><Futures /></li>
            <li class="nav-item"><Stocks /></li>
            <li class="nav-item"><Tradegatehub /></li>
          </ul>
        </div>
        <!-- Tercera sección - H2 con display: flex -->
        <div class="section d-flex flex-column flex-md-row text-center">
          <h2 class="mb-2"><Login /></h2>
          <h2 class="mb-2"><Contacto /></h2>
          <h2 class="mb-2"><Language /></h2>
        </div>
      </div>
    </div>
  </header>
</template>
