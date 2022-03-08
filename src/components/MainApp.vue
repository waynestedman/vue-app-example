<template>
<div class="main-app-content">
  <h2>{{ msg }}</h2>
  <div class="figjam">
    <h3>This FigJam illustrates the parts of a design system and how they're connected:</h3>
    <a target="_blank" href="https://www.figma.com/file/UDUmV5OdNafGKzy0zOwwa5/Design-System-exampl">
      <img src="../assets/design-system-example.png" alt="FigJam illustarting a design system">
      <caption>click to visit</caption>
    </a>
  </div>
  <div class="tokens-figma">
    <h3>It all starts by establishing your Design tokens</h3>
    <a target="_blank" href="https://www.figma.com/file/DvZ47nOktUjA0bxjUnGhgp/Design-Tokens-example">
      <p>the Figma Tokens file</p>
    </a>
  </div>
  <div class="component">
    <h3>An example of a componet, that has been built by the system</h3>
    <p>This example card is a framework agnostic web componet. It has been imported into this Vue app, the same way a UI library is used.</p>
    <p>Design Token information has flowed down to the componet and app from a single source of truth.</p>
    <card-component></card-component>
  </div>
</div>
</template>

<style lang="scss" scoped>
.main-app-content {
  margin: 1rem;

  h2 {
    font-size: var(--h2);
    margin: 0;
    // text-align: center;
  }
  a {
    // text-decoration: none;
    cursor: pointer;
    color: var(--gray-03);
    font-size: var(--body);

    caption {
      display: block;
      font-size: var(--caption);
    }
  }
  p {
    display: inline-block;
    margin: 0.5rem 0 0;
  }
  .figjam {
    display: block;
    // font-family: var(--montserrat);
    // font-size: var(--body);
    // width: 33%;
    padding: 2rem 1rem;
    margin: 2rem 0;
    background-color: #fff;
    border: 1px solid var(--gray-03);
    width: 46%;

    h3 {
      margin-top: 0;
      margin-bottom: 0.5rem;
    }
    img {
      display: block;
      width: 70%;
      height: auto;
      margin: 0 auto;
    }
  }

  .tokens-figma {
    background-color: #fff;
    width: 46%;
    margin: 2rem 0;
    padding: 1rem;
    border: 1px solid var(--gray-03);

    p {
      border-bottom: 1px solid var(--gray-03);
    }
  }

  .component {
    display: block;
    // font-family: var(--montserrat);
    // font-size: var(--body);
    background-color: #fff;
    width: 46%;
    padding: 1rem;
    border: 1px solid var(--gray-03);

    h3 {
      margin: 0.5rem 0;
    }
    // card-component {
    //   margin: 0 auto;
    // }
  }
}
</style>

<script setup>
import './card-component.js'

defineProps({
  msg: String
})

</script>
