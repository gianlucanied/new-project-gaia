<script setup></script>

<template>
  <header class="header">
    <router-link to="/">GAIA GRISANTI about</router-link>
    <router-link to="/works">works</router-link>
  </header>
</template>

<style scoped>
header {
  font-family: "Andale Mono";
  font-size: 1rem;
}

.header {
  width: 100%;
  display: flex;
  font-family: "Andale Mono";
}

a {
  text-decoration: none;
  padding: 20px;
  color: black;
}

@media (max-width: 768px) {
  a {
    padding: 10px;
    font-size: 20px;
  }
}
</style>
