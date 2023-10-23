<template>
  <div class="container-community">
    <div class="container-section-community">
      <section class="container text-center py- center-title">
        <h3>Try CommuniTraders Now!</h3>
      </section>
      <section class="container-button">
        <div class="row-a">
          <div class="col-md-6 d-flex justify-content-center">
            <div class="text-center mx-auto">
              <!-- Agregamos mx-auto para centrar horizontalmente -->
              <p class="mb-2">Free Download for Tradeview Users</p>
              <!-- Agregamos un margen inferior -->
              <button class="btn btn-danger custom-button-black">
                Contact your Broker
              </button>
            </div>
          </div>
          <div class="col-md-6 d-flex justify-content-center border-start">
            <div class="text-center mx-auto">
              <!-- Agregamos mx-auto para centrar horizontalmente -->
              <p class="mb-2">Don't have a Tradeview Account yet?</p>
              <!-- Agregamos un margen inferior -->
              <button class="btn btn-danger custom-button-red">
                Get a Free Demo
              </button>
            </div>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<style scoped>
.container-button {
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.custom-button-black {
  background-color: transparent;
}
.custom-button-red {
  background-color: #ff0000;
}
.custom-button-red:hover {
  background-color: transparent;
}
.container-community {
  background-color: #181f29;
}
.container-section-community {
  padding: 4rem;
}
.border-start {
  border-left: 1px solid #ffffff; /* Añade una línea vertical en el medio */
}
.center-title h3 {
  font-weight: 750;
  margin-top: 3rem;
  margin-bottom: 1.5rem;
  color: #ffffff;
}
.text-center {
  width: 100%;
}
.text-center p {
  color: #ffffff;
  padding: 15px;
}
.text-center p {
  color: #a2a4aa;
}
.row-a {
  display: flex;
  width: 45%;
  justify-content: center;
}
.text-center button {
  margin-bottom: 3rem;
}
@media (max-width: 768px) {
  .container-button {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  .container-section-community {
    padding: 2rem;
  }
  .text-center {
    width: 100%;
  }
  .row-a {
    display: flex;
    flex-direction: column;
    width: 100%;
    justify-content: center;
  }
}
</style>
