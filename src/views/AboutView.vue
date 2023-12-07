<script setup></script>

<template>
  <section>
    <div class="about-artist">
      <div class="cube"></div>
      <div class="about-text">
        Lorem ipsum dolor sit amet consectetur adipiscing elit nullam magnis,
        primis vehicula aenean enim nunc hendrerit pharetra platea, luctus
        facilisi nulla sociosqu accumsan dapibus diam eu. Nullam mi donec ligula
        litora himenaeos augue purus vestibulum lacus, facilisis auctor faucibus
        interdum nam fames id. Hendrerit nullam rutrum facilisis dignissim
        tristique cubilia, bibendum tempus mattis sociis.
      </div>
      <img src="/img/LogoMar.png" class="maria-logo" />
    </div>
  </section>
</template>

<style scoped>
section {
  background-color: var(--white-vintage);
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-template-rows: repeat(4, 1fr);
}
.cube {
  width: 350px;
  height: 350px;
  background-color: var(--orange-vintage);
  grid-column: 1/2;
  grid-row: 1/3;
}
.about-text {
  font-family: questrial;
  color: var(--orange-vintage);
  grid-column: 3/4;
  grid-row: 1/2;
}
.maria-logo {
  width: 100px;
}
</style>
