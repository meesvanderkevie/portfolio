<script setup>
  import { RouterLink, RouterView } from "vue-router";
  import Header from "./components/Header.vue";
</script>

<template>
  <div id="app">

    <h1 style="margin-bottom: 1px;">Hallo, ik ben Mees 👋</h1>
    <p style="color: gray; font-weight: bold;">Beginnende Developer</p>

    <a href="https://github.com/meesvanderkevie"><img src="./images/github.svg" class="img-social"></a>

    <h2>Projecten</h2>

    <p>Binnenkort meer...</p>
  </div>
</template>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Open+Sans&display=swap');

  .img-social {
    display: block;
    margin-left: auto;
    margin-right: auto;
    width: 3em;
    height: 3em;
  }

  h1 {
    font-size: 3rem;
    font-weight: bold;
    font-family: 'Open Sans', sans-serif;
    text-align: center;
  }

  h2 {
    font-size: 2rem;
    font-weight: bold;
    font-family: 'Open Sans', sans-serif;
    text-align: center;
  }

  p {
    font-size: 1.5rem;
    font-weight: semi-bold;
    font-family: 'Open Sans', sans-serif;
    text-align: center;
  }
</style>