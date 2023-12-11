<template>
  <section>
    <div class="wrapper">
      <h1 class="art-title">
        Art / Creative Projects&rarr;Experimental Fields
      </h1>
    </div>
    <div class="art-container">
      <div><img src="/img/MeditationOne.png" class="img-1 img-gallery" /></div>
      <div><img src="/img/FamilySupport.png" class="img-2 img-gallery" /></div>
      <div><img src="/img/Fauda.png" class="img-3 img-gallery" /></div>
      <div><img src="/img/HigherSelf.png" class="img-4 img-gallery" /></div>
      <div>
        <img src="/img/living in color.jpg" class="img-5 img-gallery" />
      </div>
      <div><img src="/img/underwater.png" class="img-6 img-gallery" /></div>
      <div><img src="/img/DeepSearch.png" class="img-7 img-gallery" /></div>
    </div>
    <div class="bottom">
      <p class="art-text">
        I thrive on projects that involve visual arts and various forms of
        creative expression, i see it as a way of self-exploration
        <br />
        especially in creating through analog collage.
      </p>
    </div>
    <a href="http://localhost:5173/"
      ><img src="/img/LogoMar.png" class="logo"
    /></a>
  </section>
</template>
<style>
section {
  background-color: var(--white-vintage);
}
.wrapper {
  display: flex;
  justify-content: center;
  background-color: var(--orange-vintage);
  position: sticky;
  top: 0;
}
.art-title {
  font-family: antonio;
  text-transform: uppercase;
  color: var(--white-vintage);
  font-size: 5rem;
  display: block;
}
.art-container {
  display: grid;
  place-items: center;
  grid-template-columns: 1fr 1fr;
  gap: 1rem;
}

.art-container > div {
  width: 100%;
}

img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}
.art-text {
  font-family: questrial;
  font-size: 2rem;
  text-align: center;
  color: var(--orange-vintage);
  grid-row: 6/7;
}
.bottom {
  display: flex;
  justify-content: center;
  align-content: center;
}
.logo {
  width: 10%;
  align-self: center;
  cursor: pointer;
}
</style>
