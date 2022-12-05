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
            <section
              id="dinner"
              class="section bg-image-section-one bg-vanilla block-card-section block-card-overlap"
              style="margin-top: 0px; margin-bottom: 0px"
            >
              <DinnerComponent />
            </section>
            <section
              id="spa"
              class="section block-card-section block-card-overlap bg-full-image"
            >
              <SpaComponent />
            </section>
            <section
              id="review"
              class="section our-story-summary bg-image-section-one testi"
            >
              <TestimonialComponent />
            </section>
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

.bg-image-section-one {
  position: relative;
  overflow: hidden;
}

.bg-full-image {
  padding: 0;
  min-height: 120vh;
  background-color: #000;
  position: relative;
  overflow: hidden;
}

#page_summary {
  position: relative;
  z-index: 1;
  background: #f0f0f5;
}

.our-story-summary[data-v-eab29924] {
  padding-bottom: 150px;
}
</style>
