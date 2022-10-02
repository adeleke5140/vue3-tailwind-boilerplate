<script setup>
import { RouterLink, RouterView } from 'vue-router';
</script>

<template>
  <header >
    <h1 class="text-green-400 text-3xl mx-2 my-8 text-center flex flex-col md:flex-row justify-center items-center">
    <img src="./assets/logo.svg" class="w-10 mr-4 pr-0" alt=""/>
      vue3 + <span class="text-white inline-block mx-2"> tailwindcss </span> + vue-router</h1>
    <nav class="text-white mb-16 text-center">
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
    </nav>

    
  </header>
  <footer class=" absolute bottom-0 text-green-400">
      Contribute on: <a href="https://github.com/adeleke5140" class="text-white">Github</a>
    </footer>
  <RouterView />
</template>

<style scoped>



nav a.router-link-exact-active {
  --tw-text-opacity: 1;
  color: rgb(74 222 128 / var(--tw-text-opacity));
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  margin-right: 1em;
}

</style>
