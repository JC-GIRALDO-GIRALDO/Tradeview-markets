<script setup></script>

<template>
  <div class="container-a">
    <section class="section-1">
      <article class="Contents-Part-One">
        <img
          src="https://i.imgur.com/gOY5o9N.png"
          alt="logo"
          class="logo-section-1"
        />
      </article>
    </section>
    <section class="section-2">
      <article class="container-section-2">
        <div class="centered-content">
          <div class="logo-container">
            <img
              src="https://i.imgur.com/gOY5o9N.png"
              alt="fondo"
              class="logo-image"
            />
            <div class="text-container">
              <h2>COMMUNI</h2>
              <h2>TRADERS</h2>
            </div>
          </div>
          <div class="Introduction">
            <div class="additional-text">
              <h2 class="small-text">By</h2>
              <h2 class="bottom-margin">TRADEVIEW</h2>
            </div>
            <p class="paragraph-text">
              Tradeview's CommuniTraders software lets our partners provide
              value-added copy trading to their clients.
            </p>
          </div>
          <div class="button-container">
            <div class="button-group">
              <p class="button-text">Free Download for Tradeview Users</p>
              <button class="custom-button">Contact your Broker</button>
            </div>
            <div class="button-group">
              <p class="button-text">Don't have a Tradeview Account yet?</p>
              <button class="custom-button">Get a Free Demo</button>
            </div>
          </div>
        </div>
      </article>
    </section>
  </div>
</template>

<style scoped>
/* Estilo modificado para centrar el contenido */
.container-a {
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: center; /* Centra horizontalmente el contenido */
  color: #f1f1f2;
}
.row {
  width: 100%;
}
.small-text {
  font-size: 14px;
}
.section-1 {
  width: 40%;
  height: auto;
  background-color: #dddddd;
}
.section-2 {
  width: 60%;
  background-color: #181f29;
  display: flex;
  flex-direction: column;
  justify-content: center; /* Centra verticalmente el contenido en la sección 2 */
  align-items: center; /* Centra horizontalmente el contenido en la sección 2 */
  height: 800px;
}
.centered-content {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.logo-container {
  width: 100%;
  display: flex;
  align-items: center;
}
.logo-image {
  max-width: 200px;
  margin-right: 10px;
}
.segunda-parte .text-container {
  display: flex;
  flex-direction: column;
}
bottom-margin {
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
.logo-section-1 {
  margin: 0 auto;
}
.Contents-Part-One {
  margin: 0 auto;
}
.additional-text {
  display: flex;
  flex-direction: row;
  justify-content: center;
}
container-section-2 {
  width: 100%;
  margin: 3rem auto;
}
button {
  margin-top: 10px;
}
.custom-button {
  background-color: #ff0400;
  color: #fff;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.custom-button:hover {
  background-color: #f00; /* Cambia el color de fondo al pasar el ratón sobre el botón */
}
.paragraph-text {
  text-align: center;
  font-size: 18px; /* Tamaño de fuente personalizado */
  max-width: 80%; /* Ancho máximo para un mejor diseño */
  margin: 0 auto; /* Centra el párrafo horizontalmente */
}
.button-text {
  margin: 0;
  font-size: 14px;
}
.logo-container {
  width: 100%;
  display: flex;
  justify-content: center; /* Centra horizontalmente el contenido */
  align-items: center; /* Centra verticalmente el contenido */
}

.logo-image {
  max-width: 200px;
  margin-right: 10px;
}

.text-container {
  display: flex;
  flex-direction: column;
  align-items: center; /* Centra horizontalmente el contenido */
}

.text-container h2 {
  margin-top: 10px;
}
@media (max-width: 768px) {
  .container-a {
    flex-direction: column; /* Cambia la dirección a columna en pantallas pequeñas */
  }

  .section-1 {
    width: 100%; /* Ocupa todo el ancho en pantallas pequeñas */
    height: auto; /* Ajusta la altura automáticamente según el contenido */
    margin-top: 60px; /* Agrega margen superior para dejar espacio para el menú fijo */
  }

  .section-2 {
    width: 100%; /* Ocupa todo el ancho en pantallas pequeñas */
    height: auto; /* Ajusta la altura automáticamente según el contenido */
    margin-top: 0; /* Restablece el margen superior a 0 en pantallas pequeñas */
  }
}
</style>
