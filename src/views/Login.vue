<script setup>
import { ref } from "vue";

const isDropdownOpen = ref(false);
const selectedOption = ref(null);

const toggleDropdown = () => {
  isDropdownOpen.value = !isDropdownOpen.value;
};

const selectOption = (option) => {
  selectedOption.value = option;

  isDropdownOpen.value = false;
};
</script>

<template>
  <div>
    <h2 @click="toggleDropdown">
      {{ selectedOption || "Log in" }}
      <i :class="['arrow', { open: isDropdownOpen }]"></i>
    </h2>
    <ul v-if="isDropdownOpen" class="dropdown-menu">
      <li @click="selectOption('Log in')">Log in</li>
      <li @click="selectOption('Sign up')">Sign up</li>
    </ul>
  </div>
</template>

<style scoped>
h2 {
  font-size: 15px;
  cursor: pointer;
}

.arrow::before {
  content: "▼";
  margin-left: 5px;
}

.arrow.open::before {
  content: "▲";
}

.dropdown-menu {
  border: none;
  color: #e3e3e3;
  background-color: transparent;
  list-style: none;
  padding: 0;
  display: inline;
  position: absolute;
}

.dropdown-menu li {
  padding: 5px;
  cursor: pointer;
}

.dropdown-menu a {
  text-decoration: none;
}
</style>
