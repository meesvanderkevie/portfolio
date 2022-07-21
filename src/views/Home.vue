<script>
  
  import { RouterLink, RouterView } from "vue-router";
  import Projecten from "../components/Projecten.vue";
  import Blog from "../components/Blog.vue";

  export default {
    components: {
      Projecten,
      Blog,
    },
    methods: {
      copyUsername() {
        const username = "ItzJustMees#1984";
        navigator.clipboard.writeText(username);

        alert("Copied: " + username);
      },
    }
  }
</script>

<template>

    <h1 style="margin-bottom: 1px;">Hallo, ik ben Mees 👋</h1>
    <p style="color: gray; font-weight: bold;">Beginnende Developer</p>


    <div class="social-bar">
      <a href="https://github.com/meesvanderkevie"><img src="../images/github.svg" class="img-social"></a>
      <img @click="copyUsername" src="../images/discord.svg" class="img-social">
      <a href="mailto:mvanderkevie30@gmail.com"><img src="../images/gmail.png" class="img-social"></a>
      <a href="https://discord.gg/gE4PvnvvZe"><img src="../images/Academia.jpg" class="img-social" style="border-radius: 7px;"></a>
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
    font-size: 4rem;
    font-weight: bold;
    font-family: 'Open Sans', sans-serif;
    text-align: center;
  }

  h2 {
    font-size: 2.5rem;
    font-weight: bold;
    font-family: 'Open Sans', sans-serif;
    text-align: center;
    color: rgb(0, 91, 201);
  }

  h3 {
    font-size: 1.5rem;
    font-weight: semi-bold;
    font-family: 'Open Sans', sans-serif;
    text-align: center;
    color: rgb(36, 135, 255);
  }

  p {
    font-size: 1.5rem;
    font-weight: semi-bold;
    font-family: 'Open Sans', sans-serif;
    text-align: center;
  }

  .p2 {
    font-size: 1.3rem;
    font-weight: semi-bold;
    font-family: 'Open Sans', sans-serif;
    text-align: center;
    color: rgb(0, 91, 201);
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