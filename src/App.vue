<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header></header>
  <main><RouterView /></main>
  <footer></footer>
</template>

<style scoped>
body {
  width: 100%;

  background-color: var(--white-vintage);
}
</style>
