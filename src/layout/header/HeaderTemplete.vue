<script setup>
import Forex from "../../components/Forex.vue";
import Futures from "../../components/Futures.vue";
import Stocks from "../../components/Stocks.vue";
import Login from "../../views/Login.vue";
import Contacto from "../../views/Contacto.vue";
import Language from "../../views/Language.vue";
import Tradegatehub from "../../components/Tradegatehub.vue";
</script>

<template>
  <div class="container-header">
    <!-- Primera sección - Imagen -->
    <section class="container-logo">
      <article class="content-logo">
        <img
          src="https://i.imgur.com/hctQmPu.png"
          alt="logo-tvm"
          class="logo"
        />
      </article>
    </section>
    <!-- Segunda sección - Lista con clase personalizada -->
    <section class="container-route">
      <article class="article-route">
        <h2><Forex /></h2>
        <h2><Futures /></h2>
        <h2><Stocks /></h2>
        <h2><Tradegatehub /></h2>
      </article>
    </section>
    <!-- Tercera sección - H2 con display: flex -->
    <section class="container-views">
      <article class="article-views">
        <h2><Login /></h2>
        <div class="vertical-line"></div>
        <h2><Contacto /></h2>
        <h2><Language /></h2>
      </article>
    </section>
  </div>
</template>

<style scoped>
.container-header {
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
}
.content-logo img {
  width: auto;
  margin: 2rem auto;
}
.article-route {
  width: auto;
  margin: 2rem auto;
  margin-right: 20rem;
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
}
.article-route h2 {
  cursor: pointer;
  margin-left: 20px;
  margin-right: 20px;
  font-size: 20px;
}
.article-views {
  width: auto;
  margin: 2rem auto;
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
}
.article-views h2 {
  cursor: pointer;
  margin-left: 8px;
  margin-right: 8px;
  font-size: 20px;
}
.vertical-line {
  width: 1px;
  height: 20px;
  background-color: #a2a4aa;
  margin-left: 5px;
  margin-right: 5px;
}
@media (max-width: 768px) {
  .container-header {
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  .content-logo img {
    width: auto;
    margin: 1rem auto;
  }
  .article-route {
    width: 95%;
    flex-wrap: wrap;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
  }
  .article-views {
    width: 100%;
    margin: 1rem auto;
    display: flex;
    flex-direction: row;
    justify-content: center;
  }
  .vertical-line {
    width: 1px;
    height: 15px;
  }
}
</style>
