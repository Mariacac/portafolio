<script setup>
import { ref } from "vue";
import { database } from "../database/database.js";

const showProjects = ref(database);
</script>

<template>
  <section>
    <div class="selection-window">
      <a href="http://localhost:5173/"
        ><img src="/img/LogoMar.png" class="logo"
      /></a>
      <div class="selection-title">WORK /</div>
      <div class="selection-options">
        <div class="option-one">BRANDNG</div>
        <div class="option-two">PACKAGING</div>
        <div class="option-three">POSTER DESIGN</div>
      </div>
    </div>
    <div class="work-container">
      <div v-for="(p, i) in showProjects" :key="i">
        <img
          :src="`https://drive.google.com/uc?export=view&id=${p.images}`"
          alt=""
        />
        {{ p.name }}
      </div>
    </div>
  </section>
</template>

<style scoped>
section {
  display: grid;
  grid-template-columns: max-content 1fr;
  min-height: 100vh;
  background-color: var(--white-vintage);
  width: 100%;
  background-color: var(--white-vintage);
  color: var(--orange-vintage);
  font-family: antonio;
}

.selection-window {
  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: 1fr 1fr;
  align-items: center;
  margin-left: 20px;
  justify-items: start;
}
.selection-window :hover {
  cursor: pointer;
}
.logo {
  width: 30%;
}
.selection-title {
  text-wrap: nowrap;
  font-size: 85px;
}
.selection-options {
  font-size: 40px;
  right: 60%;
}

.selection-options :hover {
  background-color: var(--orange-vintage);
  color: var(--white-vintage);
}
.work-container {
  align-self: center;
  justify-self: center;
  display: grid;
  grid-template-columns: repeat(3, 300px);
  grid-template-rows: repeat(2, 300px);
  grid-auto-rows: 300px;
  justify-content: center;
  align-content: center;
  height: 620px !important;
  overflow-y: scroll;
  height: 100%;
  gap: 20px;
}
.work-container > div {
  background-color: transparent;
}

img {
  width: 100%;
  height: 100%;
  display: block;
  object-fit: cover;
}

/*------ scrolbar ------*/
</style>
