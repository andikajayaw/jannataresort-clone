<template>
  <div>
    <!-- <LoaderComponent /> -->
    <AwardComponent />
    <div>
      <MainNavbarComponent />
      <NavbarMobileComponent v-if="isMobile" />
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
              id="page_summary"
              class="section our-story-summary bg-image-section-one testi"
              data-scroll
              data-scroll-speed="2"
            >
              <div class="q-container container-inner">
                <div class="columns type-1">
                  <div
                    id="testiTwo"
                    class="column flickity-enabled is-draggable"
                  >
                    <TestimonialComponent />
                  </div>
                </div>
              </div>
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
        if (sW >= 540) {
          return false
        } else {
          return true
        }
      } else {
        return false
      }
    },
  },
}
</script>

<style lang="scss" scoped></style>
