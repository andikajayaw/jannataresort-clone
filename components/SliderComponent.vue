<template>
  <div class="slide-inner swiper mySwiperImages">
    <div class="slides swiper-wrapper">
      <div
        v-for="(dataSlider, idx) in model.dataSlider"
        :key="idx"
        class="slide-content swiper-slide"
      >
        <div class="image-container">
          <div class="img-wrapper">
            <img
              :src="`${dataSlider.featured.aws_file_url}/${dataSlider.featured.path}/${dataSlider.featured.filename.big}`"
              alt="Slider"
            />
          </div>
        </div>
        <div class="caption">
          <h1 style="opacity: 1; transform: matrix(1, 0, 0, 1, 0, 0)">
            {{ dataSlider.title }}
          </h1>
          <div
            class="sep"
            style="opacity: 1; transform: matrix(1, 0, 0, 1, 0, 0)"
          ></div>
          <p
            style="
              opacity: 0.995257;
              transform: translate3d(0px, 0.474295px, 0px);
            "
          >
            {{ dataSlider.description }}
          </p>
          <!-- <div style="margin-top: 24px">
            <button class="btn">Read More</button>
          </div> -->
          <div
            class="link"
            style="
              opacity: 0.996805;
              transform: translate3d(0px, 0.319493px, 0px);
            "
          >
            <div class="q_magnet" style="transform: translate(0px, 0px)">
              <a class="btn">Read more</a>
            </div>
          </div>
        </div>
        <div class="grad-btm"></div>
      </div>
    </div>
    <!-- <div class="arrows">
        <div class="arrow swiper-button-next"></div>
        <div class="arrow swiper-button-prev"></div>
      </div> -->

    <div class="pagination"></div>
  </div>
</template>

<script>
import Swiper from 'swiper/swiper-bundle.min'
import 'swiper/swiper-bundle.min.css'
export default {
  data: () => {
    return {
      swipper: null,
      name: 'Component One',
      component_name: 'ComponentOne',
      model: {
        dataSlider: [
          {
            title: 'EXCLUSIVE OFFERS',
            description:
              'Discover our amazing exclusive deals and get the very best for less.',
            link: {
              title: 'Read more',
              attach: '',
              url: 'exclusive-deals',
            },
            featured: {
              id: '5e6f0fbd9dae8c6e6bb078d7',
              created_at: '2020-03-16 05:33:49',
              updated_at: '2020-03-16 05:33:49',
              updatedBy: null,
              title: null,
              description: null,
              size: 409040,
              type: 'IMG',
              original: '0a92d769-ae4f-4a86-b5d6-67fbb4bc4472.jpg',
              path: '5e65fe109dae8c14dd70f7e0/pictures/homepage/15843368292441',
              is_aws: true,
              aws_file_url:
                'https://vold-chain-hotel.s3-ap-southeast-1.amazonaws.com',
              filename: {
                big: 'big/0a92d769-ae4f-4a86-b5d6-67fbb4bc4472.jpg',
                raw: 'raw/0a92d769-ae4f-4a86-b5d6-67fbb4bc4472.jpg',
                blur: 'blur/0a92d769-ae4f-4a86-b5d6-67fbb4bc4472.jpg',
                medium: 'medium/0a92d769-ae4f-4a86-b5d6-67fbb4bc4472.jpg',
              },
            },
            id: 'a51ec325-bcfc-4bc3-8574-af2b72f7cd57',
          },
          {
            title: 'ACCOMMODATION',
            description:
              'Every accommodation has a sense of discrete luxury, combining contemporary and Balinese d??cor.',
            link: {
              title: 'Read more',
              attach: '',
              url: 'accommodation/pool-villa',
            },
            featured: {
              id: '5e72e5ab9dae8c06c7d4c21f',
              created_at: '2020-03-19 03:23:23',
              updated_at: '2020-03-19 03:23:23',
              updatedBy: null,
              title: null,
              description: null,
              size: 217067,
              type: 'IMG',
              original: 'ff642f58-71fc-4cee-9d91-d525b1c641d2.jpg',
              path: '5e65fe109dae8c14dd70f7e0/pictures/homepage/15845882025441',
              is_aws: true,
              aws_file_url:
                'https://vold-chain-hotel.s3-ap-southeast-1.amazonaws.com',
              filename: {
                big: 'big/ff642f58-71fc-4cee-9d91-d525b1c641d2.jpg',
                raw: 'raw/ff642f58-71fc-4cee-9d91-d525b1c641d2.jpg',
                blur: 'blur/ff642f58-71fc-4cee-9d91-d525b1c641d2.jpg',
                medium: 'medium/ff642f58-71fc-4cee-9d91-d525b1c641d2.jpg',
              },
            },
            id: 'a51ec325-bcfc-4bc3-8574-af2b72f7cd57',
          },
          {
            title: 'CHAMPAKA SPA ',
            description:
              'A truly luxurious experience for the senses, surrounded by the warmth of the Balinese nature.',
            link: {
              title: 'Read more',
              attach: '',
              url: 'champaka-spa',
            },
            featured: {
              id: '5e784bdd9dae8c262195e7a2',
              created_at: '2020-03-23 05:40:45',
              updated_at: '2020-03-23 05:40:45',
              updatedBy: null,
              title: null,
              description: null,
              size: 80506,
              type: 'IMG',
              original: 'e5740d7a-73ce-4643-8761-2f59c29a40f9.jpg',
              path: '5e65fe109dae8c14dd70f7e0/pictures/homepage/15849420444562',
              is_aws: true,
              aws_file_url:
                'https://vold-chain-hotel.s3-ap-southeast-1.amazonaws.com',
              filename: {
                big: 'big/e5740d7a-73ce-4643-8761-2f59c29a40f9.jpg',
                raw: 'raw/e5740d7a-73ce-4643-8761-2f59c29a40f9.jpg',
                blur: 'blur/e5740d7a-73ce-4643-8761-2f59c29a40f9.jpg',
                medium: 'medium/e5740d7a-73ce-4643-8761-2f59c29a40f9.jpg',
              },
            },
            id: 'a51ec325-bcfc-4bc3-8574-af2b72f7cd57',
          },
          {
            title: 'AMATERAS ',
            description:
              'Experience the creativity and warmth of the Balinese cuisine in our romantic setting.',
            link: {
              title: 'Read more',
              attach: '',
              url: 'amateras-dining',
            },
            featured: {
              id: '5e784bdc9dae8c262195e7a1',
              created_at: '2020-03-23 05:40:44',
              updated_at: '2020-03-23 05:40:44',
              updatedBy: null,
              title: null,
              description: null,
              size: 209987,
              type: 'IMG',
              original: '097470ab-7879-493e-bc98-5dc4fd09cb54.jpg',
              path: '5e65fe109dae8c14dd70f7e0/pictures/homepage/15849420411011',
              is_aws: true,
              aws_file_url:
                'https://vold-chain-hotel.s3-ap-southeast-1.amazonaws.com',
              filename: {
                big: 'big/097470ab-7879-493e-bc98-5dc4fd09cb54.jpg',
                raw: 'raw/097470ab-7879-493e-bc98-5dc4fd09cb54.jpg',
                blur: 'blur/097470ab-7879-493e-bc98-5dc4fd09cb54.jpg',
                medium: 'medium/097470ab-7879-493e-bc98-5dc4fd09cb54.jpg',
              },
            },
            id: 'a51ec325-bcfc-4bc3-8574-af2b72f7cd57',
          },
        ],
      },
    }
  },
  created() {
    const that = this
    this.$nextTick(() => {
      that.swipper = new Swiper('.mySwiperImages', {
        slidesPerView: 1,
        spaceBetween: 0,
        loop: true,
        freeMode: true,
        speed: 2000,
        grabCursor: true,
        watchSlidesProgress: true,
        mousewheelControl: true,
        effect: 'creative',
        creativeEffect: {
          prev: {
            // will set `translateZ(-400px)` on previous slides
            translate: [-500, 0, 0],
          },
          next: {
            // will set `translateX(100%)` on next slides
            translate: ['100%', 0, 100],
          },
        },
        autoplay: {
          delay: 2500,
          disableOnInteraction: false,
        },
        navigation: {
          nextEl: '.swiper-button-prev',
          prevEl: '.swiper-button-next',
        },
        pagination: {
          el: '.pagination',
          type: 'bullets',
          clickable: true,
        },
      })
    })
  },
}
</script>

<style lang="scss" scoped>
.image-wrapper {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-position: 50%;
  z-index: 1;
  background-size: cover;
  image-rendering: optimizeQuality;
}
</style>
