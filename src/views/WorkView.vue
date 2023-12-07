<script setup></script>

<template>
  <section>
    <div class="selection-window">
      <div class="selection-title">WORK /</div>
      <div class="selection-options">
        <div class="option-one">BRANDNG</div>
        <div class="option-two">PACKAGING</div>
        <div class="option-three">UI DESIGN</div>
      </div>
    </div>
    <div class="work-container">
      <div class="display-one"></div>
      <div class="display-two"></div>
      <div class="display-three"></div>
      <div class="display-four"></div>
      <div class="display-five"></div>
      <div class="display-six"></div>
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
}
.selection-title {
  text-wrap: nowrap;
  font-size: 85px;
}
.selection-options {
  font-size: 40px;
}
.work-container {
  display: grid;

  grid-template-columns: repeat(3, 200px);
  grid-template-rows: repeat(2, 200px);
  justify-content: center;
  align-content: center;
  width: 100%;
  height: 100%;
  gap: 20px;
}
.work-container > div {
  background-color: var(--orange-vintage);
}
</style>
