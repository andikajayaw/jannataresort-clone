<template>
  <div class="smooth">
    <div class="container">
      <section id="slider">
        <SliderComponent />
      </section>
      <section id="about">
        <ResortComponent />
      </section>
      <section id="home_accomodation">hello home_accomodation</section>
      <section id="dinner">hello dinner</section>
      <section id="spa">hello spa</section>
      <section id="review">hello review</section>
      <section id="book">hello book</section>
      <section id="footer">hello footer</section>
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>

<style lang="scss" scoped>
.smmooth {
  position: fixed;
  top: 0;
  right: 0;
  left: 0;
  width: 100%;
  height: auto;
  margin: auto;
  will-change: transform;
  z-index: 1;
}

.container {
  width: 100%;
  margin: 0 auto;
}
</style>
