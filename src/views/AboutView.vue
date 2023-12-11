<script setup></script>

<template>
  <section>
    <div class="about-title">Meet Maria</div>
    <div class="subtitle">Colombian Visual Artist and Graphic Designer</div>

    <img src="/img/Maria.jpeg" class="maria-img" />

    <div class="text">
      My work whether is a commission, digital design or into the visual art
      dimension the focus of all will always be a personal exploration, a
      journey into the intricate balance between simplicity and the profound
      nuances of the human psyche. I strive to create designs that resonate with
      emotions, inviting viewers to connect with the beauty and complexity of
      nature on a deeper level. In each piece, I carefully weave together
      elements of minimalism and psychological depth, forming a visual language
      that speaks to the soul. My portfolio is a reflection of my passion for
      translating the serene elegance of the natural world into art that goes
      beyond the visual, prompting contemplation and fostering a meaningful
      connection.
    </div>

    <a href="http://localhost:5173/"
      ><img src="/img/LogoMar.png" class="logo"
    /></a>
  </section>
</template>

<style scoped>
section {
  width: 100%;
  height: 100vh;
  background-color: var(--white-vintage);
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(2, 1fr);
  color: var(--orange-vintage);
  row-gap: 50px;
  justify-items: center;
  align-items: end;
}
.about-title {
  font-family: antonio;
  font-size: 100px;
  justify-self: center;
  align-self: center;
  grid-column: 1/2;
  grid-row: 1/2;

  text-transform: uppercase;
}
.maria-img {
  width: 50%;
  grid-column: 2/3;
  grid-row: 1/2;
  align-self: center;
  margin-top: 20px;
}
.logo {
  width: 30%;

  grid-column: 2/2;
  margin-bottom: 10px;
  cursor: pointer;
}
.subtitle {
  font-family: antonio;
  font-size: 25px;
  align-self: center;
  grid-column: 1/2;
  grid-row: 1/2;
  margin-top: 20%;
  text-align: center;
}
.text {
  font-family: questrial;
  text-align: center;
  grid-column: 2/3;
  grid-row: 2/3;
  margin-right: 25px;
  align-self: start;
}
</style>
