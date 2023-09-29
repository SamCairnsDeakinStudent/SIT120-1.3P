<script setup>
import { RouterLink, RouterView } from 'vue-router';
import FooterComponent from './components/FooterComponent.vue';
import HelloWorld from './components/FooterComponent.vue'
</script>

<template>
  <link rel="stylesheet" href="../src/assets/grid.css">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <div class="content">
    <div class="nav-container" style="background-color:black; padding-top:2vw; padding-bottom: 2vw; ">
      <div class="links-container" style="text-align:center;">
        <RouterLink class="nav-link" to="/" style="color: white; margin-right: 2vw; font-family: Arial, Helvetica, sans-serif;">Home</RouterLink>
        <RouterLink class="nav-link" to="/about" style="color: white; margin-right: 2vw; font-family: Arial, Helvetica, sans-serif;">About</RouterLink>
        <RouterLink class="nav-link" to="/contact" style="color: white; font-family: Arial, Helvetica, sans-serif;">Contact</RouterLink>
      </div>
    </div>

    <div class="page-container">
      <div class="content-wrapper">
        <RouterView />
      </div>
    </div>
    <footer class="amazing-footer" style="background-color: aquamarine;">
      <FooterComponent/>
    </footer>
  </div>
</template>

<style scoped>

</style>
