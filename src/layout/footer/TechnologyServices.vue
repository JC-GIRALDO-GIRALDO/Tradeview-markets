<template>
  <section class="container-Technology">
    <article class="text-Technology">
      <div class="info-text">
        <h3><strong>Leading Edge Technology</strong></h3>
        <p>
          Easy to use management tools, our fastest possible execution and
          spreads as low as 0.0.
        </p>
        <a href="#"><p>Quick Guide: communiTraders Web User Manual</p></a>
      </div>
    </article>
    <article class="info-Technology">
      <img
        src="../../../public/image-2.png"
        alt="imagen-tecnologia-computador-celulares"
      />
    </article>
  </section>
</template>

<style scoped>
.container-Technology {
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center; /* Centra verticalmente el contenido */
  background-color: #f2f2f2;
}

.info-Technology {
  padding: 2rem;
}
.info-Technology img {
  width: 100%;
}
.text-Technology {
  padding: 2rem;
  display: flex;
  justify-content: center;
}

.info-text {
  width: 60%;
}
.info-text h3 {
  font-size: 30px;
  margin-bottom: 2rem;
}
.info-text p {
  font-size: 20px;
}
.info-text a {
  color: black;
}
</style>
