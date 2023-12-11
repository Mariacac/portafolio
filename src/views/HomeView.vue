<script setup></script>

<template>
  <section>
    <video autoplay loop muted plays-inline class="background-video">
      <source src="/img/fusion animate_2.mp4" type="video/mp4" />
    </video>

    <img src="/img/LogoMar.png" class="logo-1" />

    <div class="side-bar">
      <div class="screens">
        <a href="" class="personal">LET'S TALK</a>
        <a href="art">ART</a>
        <a href="work">WORK</a>
        <a href="about">ABOUT</a>
      </div>
    </div>
  </section>
</template>

<style scoped>
section {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(2, 1fr);
  width: 100%;
  max-height: 100vh;
  background-color: var(--white-vintage);
  font-size: 55px;
  color: var(--orange-vintage);
  font-family: antonio;
  justify-items: center;
  overflow-x: hidden;
  overflow-y: hidden;
}

.background-video {
  display: flex;
  align-self: flex-start;
  width: 180%;
  grid-column: 2/3;
}
.logo-1 {
  grid-column: 1/2;
  grid-row: 1/2;
  width: 140px;
  justify-self: start;
  margin-top: 10px;
  margin-left: 10px;
}

.side-bar {
  grid-column: 3/4;
  display: flex;
  flex-direction: column;
}
.side-bar :hover {
  cursor: pointer;
}
.side-bar a {
  display: flex;
  flex-direction: column;
  text-decoration: none;
  color: var(--orange-vintage);
}
.screens :hover {
  background-color: var(--orange-vintage);
  color: var(--white-vintage);
}
.personal:hover {
  background-color: var(--orange-vintage);
  color: var(--white-vintage);
  width: 200px;
}

.screens {
  z-index: 100 !important;
}
.screens a {
  cursor: pointer;
}
</style>
