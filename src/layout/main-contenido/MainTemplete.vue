<script setup></script>

<template>
  <div class="container-main-intro">
    <section class="section-img">
      <img
        src="https://i.imgur.com/U45qgw4.png"
        alt="logo"
        class="logo-section-1"
      />
    </section>
    <section class="section-text-intro">
      <article class="section-article-intro">
        <div class="logo-container">
          <img
            src="https://i.imgur.com/ha9yFmm.png"
            alt="logo-communi"
            class="logo-image"
          />
        </div>
      </article>
      <article class="section-article-text">
        <div class="centered-content">
          <hr />
          <p class="paragraph-text">
            Tradeview's <strong>CommuniTraders</strong> software lets our
            partners provide value-added copy trading to their clients.
          </p>
        </div>
      </article>
      <article class="section-article-button">
        <div class="button-container">
          <div class="button-group">
            <p class="button-text">Free Download for Tradeview Users</p>
            <button class="custom-button button-1">Contact your Broker</button>
          </div>
          <div class="vertical-line"></div>
          <div class="button-group">
            <p class="button-text">Don't have a Tradeview Account yet?</p>
            <button class="custom-button button-2">Get a Free Demo</button>
          </div>
        </div>
      </article>
    </section>
  </div>
</template>

<style scoped>
/* Estilo modificado para centrar el contenido */
.container-main-intro {
  width: 100%;
  display: flex;
  flex-direction: row;
  max-height: 900px;
  background-color: #e3e3e3;
}
.section-img {
  width: 40%;
}
.section-img img {
  width: 100%;
  height: 100%;
}
.section-text-intro {
  width: 60%;
  background-color: #181f29;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.centered-content {
  width: 70%;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.centered-content p {
  max-width: 80%;
  margin: 0 auto;
  border-top: 2px solid #a2a4aa;
  font-size: 33px;
  text-align: center;
  color: #a2a4aa;
}
.centered-content strong {
  color: #ffffff;
}
.section-article-intro {
  width: 100%;
  margin: 2rem auto;
}
.logo-container {
  width: 100%;
  height: auto;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.logo-container img {
  width: 30%;
  margin: 0 auto;
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
  margin-top: 25px;
}
.custom-button {
  background-color: #ff0400;
  color: #fff;
  padding: 10px 20px;
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.button-text {
  color: #a2a4aa;
  margin: 0;
  font-size: 15px;
}
.button-1 {
  background-color: transparent;
}
.button-2:hover {
  background-color: rgba(255, 255, 255, 0.178);
}
.custom-button:hover {
  background-color: rgba(255, 255, 255, 0.178);
}
.vertical-line {
  width: 1px;
  height: 100px;
  background-color: #a2a4aa;
  margin-left: 40px;
  margin-right: 40px;
}
@media (max-width: 768px) {
  .container-main-intro {
    width: 100%;
    display: flex;
    flex-direction: column;
  }
  .section-img {
    width: 100%;
  }
  .section-img img {
    width: 100%;
    height: 100%;
  }
  .section-text-intro {
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .section-article-intro {
    width: 100%;
    margin: 2rem auto;
  }
  .logo-container img {
    width: 50%;
    margin: 0 auto;
  }
  .button-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 20px;
  }
  .button-group {
    display: flex;
    flex-direction: column;
    padding: 20px;
  }
  .vertical-line {
    width: 0;
    height: 0;
    margin-left: 0;
    margin-right: 0;
  }
}
</style>
