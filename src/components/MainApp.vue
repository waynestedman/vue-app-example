<template>
<h1>{{ msg }}</h1>
<div class="main-app-content">
  <div class="figjam concept">
    <h2>This FigJam illustrates the parts of a design system and how they're connected:</h2>
    <a target="_blank" href="https://www.figma.com/file/UDUmV5OdNafGKzy0zOwwa5/Design-System-example">
      <img src="../assets/tokens-pipeline-diagram.png" alt="FigJam illustarting a design system">
      <p>click to see the FigJam diagram</p>
    </a>
  </div>
  <div class="tokens-figma concept">
    <h2>#1 - It all starts by establishing your Design tokens</h2>
    <a target="_blank" href="https://www.figma.com/file/DvZ47nOktUjA0bxjUnGhgp/Design-Tokens-example">
      <img src="../assets/tokens-in-figma.png" alt="Figma file for the Dsign Tokens">
      <p>click to see the Figma Tokens file</p>
    </a>
  </div>
  <div class="component concept">
    <h2>#2 - An example of a componet,<br>that has been built by the system</h2>
    <p>This example card is a framework agnostic web componet. It has been imported into this Vue app, exactly the same way any other UI library is used.</p>
    <p>Design Token information has flowed down to the componet and app from the single source of truth.</p>
    <card-component></card-component>
  </div>
  <div class="vue-app concept">
    <h2>#3 - the Result is an app like this one</h2>
    <a target="_blank" href="https://github.com/waynestedman/vue-app-example">
      <img src="../assets/vue-app-github.png" alt="Vue App Github repository">
      <p>click to see the repo for this Vue App</p>
    </a>
  </div>
</div>
</template>

<style lang="scss" scoped>
h1 {
  font-size: var(--h1);
  margin: 1rem;
  // text-align: center;
}

.main-app-content {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-between;
  margin: 0 1rem;

  a {
    cursor: pointer;
    color: var(--gray-03);
    font-size: var(--body);

    p {
      display: block;
      font-size: var(--body);
      text-align: center;
    }
  }
  
  p {
    display: inline-block;
    margin: 0.5rem 0 0;
  }

  .concept {
    display: inline-block;
    padding: 1rem;
    margin: 1rem 0;
    background-color: #fff;
    // border: 1px solid var(--gray-03);
    border-radius: 8px;
    max-width: 46%;

    h2 {
      margin-top: 0;
      margin-bottom: 0.5rem;
    }

    img {
      display: block;
      width: 70%;
      height: auto;
      margin: 0 auto;
    }
  } // concept
  .figjam h2 {
    max-width: 75%;
  }
} // main-app-content
</style>

<script setup>
import './card-component.js'

defineProps({
  msg: String
})

</script>
