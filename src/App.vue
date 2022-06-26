<script>
  
  import { RouterLink, RouterView } from "vue-router";
  import Header from "./components/Header.vue";

  export default {
    components: {
      Header
    },
    methods: {
      copyUsername() {
        const username = "ItzJustMees#1984";
        navigator.clipboard.writeText(username);

        alert("Copied: " + username);
      }
    }
  }
</script>

<template>
  <div id="app">

    <Header/>

    <h1 style="margin-bottom: 1px;">Hallo, ik ben Mees 👋</h1>
    <p style="color: gray; font-weight: bold;">Beginnende Developer</p>

    <div class="social-bar">
      <a href="https://github.com/meesvanderkevie"><img src="./images/github.svg" class="img-social"></a>
      <img @click="copyUsername" src="./images/discord.svg" class="img-social">
      <a href="mailto:mvanderkevie30@gmail.com"><img src="./images/gmail.png" class="img-social"></a>
      <a href="https://discord.gg/gE4PvnvvZe"><img src="./images/Academia.jpg" class="img-social" style="border-radius: 7px;"></a>
    </div>
  </div>
</template>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Open+Sans&display=swap');

  .img-social {
    display: block;
    width: 4em;
    height: 4em;
    transition: all 0.4s ease-in-out;
  }

  .img-social:hover {
    width: 4.5em;
    height: 4.5em;
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

  .social-bar {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 1rem;
  }
</style>