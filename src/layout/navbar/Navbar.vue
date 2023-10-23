<template>
  <div>
    <nav class="navbar">
      <!-- Botón de menú para pantallas pequeñas -->
      <button class="menu-button" @click="toggleMenu">☰</button>
      <ul class="navbar-list" :class="{ 'menu-open': isMenuOpen }">
        <li class="navbar-item"><a href="#">Markets</a></li>
        <li class="navbar-item"><a href="#">Company ▼</a></li>
        <li class="navbar-item"><a href="#">Accounts</a></li>
        <li class="navbar-item"><a href="#">Platforms ▼</a></li>
        <li class="navbar-item"><a href="#">Pricing</a></li>
        <li class="navbar-item"><a href="#">Introducing Brokers</a></li>
        <li class="navbar-item"><a href="#">Education</a></li>
        <li class="navbar-item"><a href="#">Support ▼</a></li>
      </ul>
    </nav>
  </div>
</template>

<script setup>
import { ref } from "vue";

const isMenuOpen = ref(false);

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
};
</script>

<style scoped>
.menu-button {
  font-size: 20px;
  cursor: pointer;
  display: none;
  background-color: transparent;
  text-decoration: none;
  color: #ff0400;
}
.navbar-list {
  list-style: none;
  display: flex;
  margin: 0;
  padding: 0;
}
.navbar-item {
  margin-bottom: 1rem;
  margin-top: 1.5rem;
  margin-left: 25px;
  margin-right: 25px;
}
.navbar-item a {
  color: #f1f1f2;
  text-decoration: none;
  margin-left: 20px;
  margin-right: 20px;
}
.menu-open {
  display: none;
  flex-direction: column;
  background-color: #181f29;
  position: absolute;
  top: 50px;
  right: 0;
  z-index: 1;
  transition: right 0.3s;
}
.menu-open li {
  padding: 10px;
}

@media (max-width: 768px) {
  .menu-button {
    display: block;
  }
  .navbar-list {
    display: flex;
    flex-direction: column;
  }
  .navbar-item {
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;
    justify-content: center;
    flex-wrap: wrap;
  }
  .menu-open {
    right: -250px;
  }
}
</style>
