<template>
  <h1>{{ msg }}</h1>
  <card-component></card-component>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>

<script setup>
// import './web-components-example.es.js'
import './card-component.js'

defineProps({
  msg: String
})

</script>
