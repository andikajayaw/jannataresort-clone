<template>
  <div>
    <!-- <LoaderComponent /> -->
    <AwardComponent />
    <div>
      <MainNavbarComponent />
      <NavbarMobileComponent v-if="!isMobile" />
    </div>
    <SmoothScrool>
      <div data-scroll-section class="smooth loco-scroll">
        <HeaderComponent />
        <div>
          <div class="container">
            <section
              id="slider"
              class="slide"
              data-scroll
              data-scroll-speed="2"
            >
              <SliderComponent />
            </section>
            <section
              id="about"
              class="section block-card-section bg-vanilla bg-image-section-one"
              style="margin-top: 0px; margin-bottom: 0px"
              data-scroll
              data-scroll-speed="2"
            >
              <ResortComponent />
            </section>
            <section
              id="home-accomodation"
              style="padding: 150px 0; margin-top: 0px; margin-bottom: 0px"
              class="section block-fullscreen bg-blue-dark bg-image-section-two"
              data-scroll
              data-scroll-speed="2"
            >
              <AccomodationComponent />
            </section>
            <section
              id="dinner"
              class="section bg-image-section-one bg-vanilla block-card-section block-card-overlap"
              data-scroll
              data-scroll-speed="2"
            >
              <DinnerComponent />
            </section>
            <section
              id="spa"
              class="section block-card-section block-card-overlap bg-full-image"
              data-scroll
              data-scroll-speed="2"
              style="margin-top: 0px; margin-bottom: 0px"
            >
              <SpaComponent />
            </section>
            <section
              id="review"
              class="section our-story-summary bg-image-section-one testi"
              data-scroll
              data-scroll-speed="2"
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
export default {
  name: 'IndexPage',
  data: () => {
    return {}
  },
  computed: {
    isMobile() {
      if (process.client) {
        const sW = window.innerWidth
        if (sW <= 545) {
          return true
        } else {
          return false
        }
      } else {
        return false
      }
    },
  },
  // created() {
  //   const sW = window.screen.width
  //   if (sW <= 540) {
  //     this.isMobile = true
  //   }
  // },
}
</script>

<style lang="scss" scoped>
#page_summary {
  position: relative;
  z-index: 1;
  background: #f0f0f5;
}

.our-story-summary {
  padding-bottom: 150px;
}
</style>
