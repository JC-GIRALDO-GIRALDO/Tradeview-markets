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
  <header class="header-container">
    <div class="row align-items-center">
      <!-- Primera sección - Imagen -->
      <section class="container-logo col-lg-3 col-md-3 col-sm-6">
        <article class="content-logo">
          <img
            src="https://i.imgur.com/gOY5o9N.png"
            alt="logo-tvm"
            class="logo"
          />
        </article>
        <article class="content-name">
          <div>
            <h1>
              <span class="primer-nombre">TRADE</span
              ><span class="segundo-nombre">VIEW</span>
            </h1>
          </div>
          <div>
            <h2>MARKETS</h2>
          </div>
        </article>
      </section>
      <!-- Segunda sección - Lista con clase personalizada -->
      <section class="container-rutas col-lg-6 col-md-6 col-sm-6">
        <ul class="nav navigation-menu justify-content-center">
          <li><Forex /></li>
          <li><Futures /></li>
          <li><Stocks /></li>
          <li><Tradegatehub /></li>
        </ul>
      </section>
      <!-- Tercera sección - H2 con display: flex -->
      <section
        class="col-lg-3 col-md-3 col-sm-12 d-flex justify-content-end section"
      >
        <h2><Login /></h2>
        <h2><Contacto /></h2>
        <h2><Language /></h2>
      </section>
    </div>
  </header>
</template>

<style scoped>
.header-container {
  width: 100%;
  color: #f1f1f2;
  padding: 10px 0;
}

.container-logo {
  display: flex;
  flex-direction: row;
  align-items: center;
}
.container-rutas {
  display: flex;
  flex-direction: initial;
}
.primer-nombre {
  color: #f1f1f2;
}

.segundo-nombre {
  color: #ff0400;
}

.content-name h1 {
  font-size: 25px;
}

.content-name h2 {
  font-size: 15px;
  margin-top: -10px;
}

.content-logo img {
  width: 100px;
  margin-top: -22px;
}

.section {
  flex: 1;
  padding: 10px;
}

.section h2 {
  margin-left: 10px;
  margin-right: 10px;
  cursor: pointer;
}

.logo {
  max-width: 100%;
}

.navigation-menu {
  list-style: none;
  display: flex;
  justify-content: center;
}

.nav-item {
  margin: 0 10px;
}

h2 {
  margin: 0;
}

.nav li {
  margin-left: 20px;
  margin-right: 20px;
  cursor: pointer;
}

/* Ajustes para pantallas pequeñas */
@media (max-width: 768px) {
  .col-sm-6 {
    flex: 1;
  }
}
/* Añade estilos para pantallas pequeñas */
@media (max-width: 768px) {
  .header-container {
    margin: 0 auto;
    flex-direction: column; /* Cambia la dirección del contenedor principal a columna */
    align-items: center; /* Centra los elementos en la columna */
  }

  .container-logo,
  .container-rutas,
  .section {
    margin: 0 auto;
    width: 100%; /* Haz que estos elementos ocupen el 100% del ancho */
    text-align: center;
  }

  .navigation-menu {
    color: #ff0400;
    display: flex;
    flex-direction: column; /* Coloca los elementos de la lista en una columna */
  }

  .nav li {
    margin: 5px 0; /* Aumenta el espacio entre los elementos de la lista */
  }
}
/* Ajustes para pantallas pequeñas */
@media (max-width: 768px) {
  .content-logo img {
    width: auto;
  }

  .section {
    width: 100%;
    padding: 20px;
  }

  .section h2 {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: center;
  }
}
</style>
