<script setup>

</script>

<template>
  <header class="header">
      <router-link to="/">GAIA GRISANTI</router-link>
      <router-link to="/works">WORKS</router-link>
  </header>
</template>

<style scoped>
header {
  font-family: 'Andale Mono';
  font-size: 1rem;
}

.header {
  width: 100%;
  background-color: black;
  display: flex;
  justify-content:space-between;
  font-family: 'Andale Mono';
}

a {
  text-decoration: none;
  color: white;
  padding: 20px;
}

@media (max-width: 768px) {
  a {
    padding: 10px;
    font-size: 20px;
  }
}
</style>
