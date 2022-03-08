<script setup>
import MainApp from './components/MainApp.vue'
</script>

<template>
  <header>
    <h1>This is a Design System Powered Web App</h1>
  </header>
  <main-app msg="Tokens to App, how does it work?" />
</template>

<style lang="scss">
header {
  background-color: var(--teal-03);
  color: #fff;
  margin: 0;
  text-align: center;
}
h1 {
  font-family: var(--raleway);
  font-size: var(--h1);
  padding: 1rem;
  margin: 0;
}

#app {
}
</style>
