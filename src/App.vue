<script setup>
import MainApp from './components/MainApp.vue'
</script>

<template>
  <header>
    <h2>Vue app - styled by Design Tokens</h2>
  </header>
  <main-app msg="Example web component" />
</template>

<style lang="scss">
header {
  background-color: var(--teal-03);
  color: var(--gray-02);
  margin: 0;
}
h2 {
  font-family: var(--raleway);
  font-size: var(--h3);
  padding: 1rem;
  margin: 0;
}

// #app {
  
// }
</style>
