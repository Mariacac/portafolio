<script setup></script>

<template>
  <section>
    <video autoplay loop muted plays-inline class="background-video">
      <source src="/img/fusion_animate_2.mp4" type =video/mp4>
    </video>
    <img src="/img/LogoMar.png" class="logo" />
    <div class="side-bar">
      <div class="contact-btn">LET'S TALK</div>

      <div class="screens">
        <div class="work-screen">WORK</div>
        <div class="collage-screen">COLLAGE</div>
        <div class="about-screen">ABOUT</div>
      </div>
    </div>
  </section>
</template>

<style scoped>
section {
  display: grid;

  grid-template-columns: repeat(6, 1fr);
  grid-template-rows: repeat(6, 1fr);
  width: 100%;
  background-color: var(--white-vintage);
  font-size: 35px;
  color: var(--orange-vintage);
  font-family: antonio;
  justify-content: space-between;
}

.background-video {
  grid-row: 1/3;
  grid-column: 2/2;
  justify-self: center;
}
.logo {
  grid-row: 1/2;
  grid-column: 1/2;
  width: 180px;
}

.side-bar {
  display: grid;
  grid-template-columns: repeat(1, fr);
  grid-template-rows: repeat(3, 1fr);
  justify-items: end;
}
.screens {
  grid-row: 3/4;
  grid-column: 1/2;

  align-self: end;
}
.contact-btn {
  grid-row: 1/2;
  grid-column: 1/2;
}

.screens > div {
  cursor: pointer;
}
</style>
