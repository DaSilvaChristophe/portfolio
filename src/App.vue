<script setup>

  import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <div id="app" class="bg-light">
    <RouterLink to="/"></RouterLink>
    <RouterView />
  </div>
</template>

<style>

  #app {
    width: 100%;
    height: auto;
    margin: 0 auto;
    padding: 0;
    box-sizing: border-box;
    display: grid;
    grid-template-columns: 1fr;
  }
  
</style>
