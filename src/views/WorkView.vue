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
  background-color: var(--white-vintage);
  width: 100%;
  background-color: var(--white-vintage);
  color: var(--orange-vintage);
  font-family: antonio;
}
.selection-window {
  display: grid;
  grid-template-columns: repeat(1, 1fr);
  grid-template-rows: repeat(2, 1fr);
  justify-content: start;
}
.selection-title {
  font-size: 85px;
  grid-column: 1/2;
  grid-row: 1/2;
}
.selection-options {
  font-size: 40px;
  grid-column: 1/2;
  grid-row: 2/3;
}
.work-container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(2, 1fr);
  background-color: var(--orange-vintage);
  width: 160px;
  height: 160px;
  justify-content: end;
}
.display-one {
  grid-row: 1/2;
  grid-column: 1/2;
}
.display-two {
  grid-row: 1/2;
  grid-column: 2/3;
}
.display-three {
  grid-row: 1/2;
  grid-column: 2/4;
}
.display-four {
  grid-row: ;
  grid-column: ;
}
.display-five {
  grid-row: ;
  grid-column: ;
}
.display-six {
  grid-row: ;
  grid-column: ;
}
</style>
