<template>
  <div>
    <SmoothScrool>
      <!-- <LoaderComponent /> -->
      <AwardComponent />
      <div
        class="smooth loco-scroll div-smooth"
        style="
          transform: matrix3d(1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
          opacity: 1;
          pointer-events: all;
        "
      >
        <HeaderComponent />
        <div>
          <div class="container">
            <section id="slider" class="slide">
              <SliderComponent />
            </section>
            <section
              id="about"
              class="section block-card-section bg-vanilla bg-image-section-one"
              style="margin-top: 0px; margin-bottom: 0px"
            >
              <ResortComponent />
            </section>
            <section
              id="home-accomodation"
              style="padding: 150px 0; margin-top: 0px; margin-bottom: 0px"
              class="section block-fullscreen bg-blue-dark bg-image-section-two"
            >
              <AccomodationComponent />
            </section>
            <section id="dinner">hello dinner</section>
            <section id="spa">hello spa</section>
            <section id="review">hello review</section>
            <section id="book">hello book</section>
            <section id="footer">hello footer</section>
          </div>
        </div>
      </div>
    </SmoothScrool>
  </div>
</template>

<script>
// import LocomotiveScroll from 'locomotive-scroll'
export default {
  name: 'IndexPage',
  data: () => {
    return {
      scroll: null,
    }
  },
  created() {
    // this.locomotiveScrollInit()
  },
  methods: {
    locomotiveScrollInit() {
      this.scroll = new this.$LocomotiveScroll({
        el: document.querySelector('[data-scroll-container]'),
        smooth: true,
        getDirection: true,
      })
      this.scroll.stop()
    },
  },
}
</script>

<style lang="scss" scoped>
.div-smooth {
  transform: matrix3d(1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
  opacity: 1;
  pointer-events: all;
}
.section {
  padding: 150px 0 100px;
}
</style>
