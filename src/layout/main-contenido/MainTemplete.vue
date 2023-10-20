<script setup></script>
<template>
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <section class="section-1">
          <article>
            <img src="../../../public/logo.png" alt="logo">
          </article>
        </section>
      </div>
      <div class="col-md-6 d-flex align-items-center justify-content-center">
        <section class="section-2">
          <article>
            <div class="logo-container">
              <img src="../../../public/logo.png" alt="fondo" class="img-fluid logo-image">
              <div class="text-container">
                <h2>COMMUNI</h2>
                <h2>TRADERS</h2>
              </div>
              
            </div>
            <div class="additional-text">
              <h2 class="small-text">By</h2>
              <h2 class="bottom-margin">TRADEVIEW</h2>
            </div>

            <div class="button-container">
              <div class="button-group">
                <p>Free Download for Tradeview Users</p>
                <button>Contact your Broker</button>
              </div>
              <div class="button-group">
                <p>Don't have a Tradeview Account yet?</p>
                <button>Get a Free Demo</button>
              </div>
              <!-- Agrega más contenido aquí si es necesario -->
            </div>
          </article>
        </section>
      </div>
    </div>
  </div>
</template>

<style scoped>
/* Estilo original */
.container {
  width: 100%;
  display: flex;
}
.row {
  width: 100%;
}
.small-text {
  font-size: 14px;
}

.logo-container {
  display: flex;
  align-items: center;
}

.logo-image {
  max-width: 200px;
  margin-right: 10px;
}

.text-container {
  display: flex;
  flex-direction: column;
}

.additional-text {
  display: flex;
  align-items: center;
  text-align: center;
  margin-top: 10px;
}

.bottom-margin {
  margin-top: 5px;
}

.button-container {
  display: flex;
  align-items: center;
  margin-top: 20px;
}

.button-group {
  display: flex;
  flex-direction: column;
  padding: 20px;
}

button {
  margin-top: 10px; /* Ajusta el margen superior según tus necesidades */
}
</style>
