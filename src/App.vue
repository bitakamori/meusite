<script>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <header>
    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/works">Escolaridade</RouterLink>
      <RouterLink to="/tec">Hobbies</RouterLink>
      <RouterLink to="/about">About Me</RouterLink>
    </nav>
  </header>

  <RouterView />
</template>



<style scoped>
  header {
    line-height: 1.5;

    padding-top: 40px;
    padding-bottom: 20px;
  }


  nav {
    width: 100%;
    font-size: 12px;
    text-align: center;
    margin-top: 0rem;
    font-weight: 200;

    /* border: 1px solid red; */

  }

  nav a.router-link-exact-active {
    color: var(--color-text);
  }

  nav a.router-link-exact-active:hover {
    background-color: transparent;
    font-weight: 400;

  }

  nav a {
    display: inline-block;
    padding: 0 1rem;
    border-left: 1px solid var(--color-border);
  }
</style>
