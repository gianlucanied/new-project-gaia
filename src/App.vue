<script setup>
import Home from './views/Home.vue'
import Works from './views/Works.vue'
import Header from './components/Header.vue'


</script>

<template>
<Header></Header>
  <router-view />
</template>


<style>
body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
