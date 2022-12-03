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
              'Every accommodation has a sense of discrete luxury, combining contemporary and Balinese décor.',
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
        spaceBetween: 13,
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
.swiper {
  width: 100%;
  height: 100%;
}

.swiper-slide {
  text-align: center;
  font-size: 18px;
  background: #fff;

  /* Center slide text vertically */
  display: -webkit-box;
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  -webkit-justify-content: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  -webkit-align-items: center;
  align-items: center;
  min-height: 745px !important;
}

.swiper-slide img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
  height: 745px !important;
}

.slide .slide-inner {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.slide .slides {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.slide .image-container {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-position: 50%;
  z-index: 1;
  background-size: cover;
}
.slide .image-wrapper {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-position: 50%;
  z-index: 1;
  background-size: cover;
}

.slide .slide-content {
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 2;
  color: #fff;
  display: flex;
  justify-content: center;
  align-items: center;
}

.slide .slide-content .caption {
  z-index: 1;
  color: white !important;
  position: absolute;
  left: 50%;
  bottom: 15%;
  width: 70%;
  // max-width: 480px;
  text-align: center;
  transform: translateX(-50%) translateY(0);
}

.slide .slide-content .caption h1 {
  font: 400 43px/1.3 Playfair Display, serif;
  margin-top: 0;
  text-transform: uppercase;
  margin-bottom: 0;
  letter-spacing: 5px;
}

.slide .slide-content .caption p {
  font: 400 14px/1.8 Open Sans, sans-serif;
  max-width: 400px;
  letter-spacing: 1px;
  margin: 30px auto 0;
}

.slide .slide-content .sep {
  width: 80px;
  height: 1px;
  background-color: hsla(0, 0%, 100%, 0.8);
  margin: 30px auto;
  display: none;
}

.btn {
  display: inline-block;
  border: 1px solid #fff;
  padding: 10px 30px;
  color: #fff;
  font: 400 11px/1.3 Open Sans, sans-serif;
  text-transform: uppercase;
  letter-spacing: 2px;
  transition: all 0.2s ease;
}

.q_magnet {
  padding: 50px 20px 20px;
  display: inline-block;
}

.btn {
  background: 0 0;
}

.btn:hover {
  background-color: #fff;
  color: #000;
}

.pagination {
  position: absolute;
  left: 10%;
  cursor: default;
  z-index: 2;
  bottom: 10%;
  margin-top: -56px;
}
.swiper-button-prev {
  margin-right: 70px;
}

.arrows {
  display: block;
  // padding: 20px;
  position: absolute;
  bottom: 14%;
  margin-bottom: -20px;
  cursor: pointer;
  z-index: 3;
  right: 10%;
}

.swiper-button-next:after,
.swiper-rtl .swiper-button-prev:after {
  content: 'prev';
}

.swiper-button-prev:after,
.swiper-rtl .swiper-button-prev:after {
  content: 'next';
}

.swiper-pagination-bullet {
  position: relative;
  display: inline-block;
  cursor: pointer;
  text-indent: -999em;
  z-index: 1;
  margin: 0 15px;
}

.grad-btm {
  position: absolute;
  z-index: 1;
  left: 0;
  width: 100%;
  bottom: 0;
  height: 40%;
  pointer-events: none;
  background: linear-gradient(180deg, transparent 0, rgba(0, 0, 0, 0.65));
}
</style>
