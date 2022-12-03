<template>
  <div>
    <LoaderComponent />
    <AwardComponent />
    <div class="smooth loco-scroll div-smooth">
      <HeaderComponent />
      <div>
        <div class="container">
          <section id="slider" class="slide">
            <SliderComponent />
          </section>
          <section
            id="about"
            class="bg-img-section-one"
            style="margin-top: 0px; margin-bottom: 0px"
          >
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
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>

<style lang="scss" scoped>
.div-smooth {
  transform: matrix3d(1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  opacity: 1;
  pointer-events: all;
}

.bg-image-section-one {
  position: relative;
  overflow: hidden;
}
</style>
