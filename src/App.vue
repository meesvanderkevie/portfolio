<script>
  
  import { RouterLink, RouterView } from "vue-router";
  import Header from "./components/Header.vue";

  export default {
    components: {
      Header
    }
  }
</script>

<template>
  <div id="app">

    <Header/>

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
    transition: all 0.4s ease-in-out;
  }

  .img-social:hover {
    width: 3.5em;
    height: 3.5em;
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

  a {
    text-decoration: none;
    color: rgb(0, 65, 149);
  }
</style>