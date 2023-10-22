<script setup>
// Importa tus imágenes aquí si es necesario
// import plantImage from "./plant.png";
// import candadoImage from "./candado.png";
// import magicImage from "./magic.png";
// import tocImage from "./toc.png";
// import awardImage from "./award.png";

const Service = [
  {
    title: "Ideal for Beginner Clients",
    description:
      "Increase trading volumes as new traders gain comfort by following successful traders in forex markets and beyond into stocks, options, commodities, and more…",
    image: "imagen",
  },
  {
    title: "Low Barriers to Entry",
    description:
      "CommuniTraders software is free and clients can start with just a $100 minimum investment.",
    image: "imagen",
  },
  {
    title: "Simple Interface",
    description:
      "A simple GUI provides needed features and tools but isn’t bogged down by non-core features. This allows clients to get set up quickly and start trading.",
    image: "imagen",
  },
  {
    title: "No Long-Term Commitments",
    description:
      "Clients can easily sign up to start, change signal providers, or stop the service. There is no long-term lockup.",
    image: "imagen",
  },
  {
    title: "Funds Safety",
    description:
      "CommuniTraders benefits from the same strong regulation and banking partners standalone Tradeview clients enjoy along with transparency and negative balance protection.",
    image: "imagen",
  },
  {
    title: "Tradeview Runs CommuniTrader",
    description:
      "You will experience the Tradeview service you know and love, no gimmicks or hidden fees, excellent live customer support, and your dedicated account manager.",
    image: "imagen",
  },
];
</script>

<template>
  <div class="container my-4 p-3">
    <div class="row">
      <div
        v-for="(service, index) in Service"
        :key="index"
        class="col-md-4 mb-4 d-flex"
      >
        <div class="card">
          <img :src="service.image" class="card-img-top" alt="Service Image" />
          <div class="card-body">
            <h5 class="card-title red-text">{{ service.title }}</h5>
            <p class="card-text">{{ service.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  color: #ffffff;
}
.row {
  margin-top: 2rem;
  margin-bottom: 2rem;
}
/* Aplicar sombreado o difuminado en lugar de borde */
.card {
  background-color: #ffffff;
  border: none;
  box-shadow: 5px 5px 15px 10px #f8f8f8;
}

/* Cambiar el color del título a rojo */
.red-text {
  color: red;
}
@media (max-width: 768px) {
  .container {
  width: 100%;
}
.row {
  width: 100%;
}
/* Aplicar sombreado o difuminado en lugar de borde */
.card {
 width: 100%;
}

}
</style>
