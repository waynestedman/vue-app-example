<template>
<div class="main-app-content">
  <h1>{{ msg }}</h1>
  <div class="content-copy">
    <p>This example card is a framework agnostic web componet. It has been imported into this Vue app, the same way a UI library is used.</p>
    <p>Design Token information has flowed down to the componet and app from a single source of truth.</p>

  </div>
  <card-component></card-component>
</div>
</template>

<style lang="scss" scoped>
.main-app-content {
  margin: 1rem;

  h1 {
    font-size: var(--h1);
    margin: 0;
  }
  .content-copy {
    display: inline-block;
    font-family: var(--montserrat);
    font-size: var(--body);
    width: 33%;
  }
}
</style>

<script setup>
import './card-component.js'

defineProps({
  msg: String
})

</script>
