<template>
  <div class="q-container container-inner">
    <!-- <div class="columns type-1">
      <div class="column flickity-enabled is-draggable">
        <div
          class="swipper flickity-viewport"
          style="height: 287px; touch-action: pan-y"
        >
          <div
            class="swiper-wrapper flickity-slider"
            style="left: 0px; transform: translate3d(-400%, 0px, 0px)"
          >
            <div
              v-for="slider in model.dataSlider"
              :key="slider.id"
              class="slide swiper-slide"
              style="position: absolute; left: 0%"
              aria-hidden="true"
            >
              <p>
                {{ slider.description }}
              </p>
              <small>{{ slider.title }}</small>
            </div>
          </div>
        </div>
      </div>

    </div> -->
    <div class="swiper mySwiper">
      <div class="swiper-wrapper">
        <div
          v-for="slider in model.dataSlider"
          :key="slider.id"
          class="swiper-slide"
          aria-hidden="true"
        >
          <p>
            {{ slider.description }}
          </p>
          <br />
          <small>{{ slider.title }}</small>
        </div>
      </div>
      <div class="swiper-button-next"></div>
      <div class="swiper-button-prev"></div>
      <div class="swiper-pagination"></div>
    </div>
  </div>
</template>

<script>
import Swiper from 'swiper/swiper-bundle.min'
import 'swiper/swiper-bundle.min.css'
export default {
  data: () => {
    return {
      swipper: null,
      name: 'Component Six',
      component_name: 'ComponentSix',
      model: {
        dataSlider: [
          {
            title: ' — Sara B, Germany',
            description:
              'This hotel is just so beautiful and peaceful. The staff is amazing, very kind and competent, always with a smile on their face and always there for you. The room we were in was beautiful, clean, very big. The bathroom was to die for, and the view breathtaking.',
            id: 'e19d53e1-999c-4703-8aef-7265f886531d',
          },
          {
            title: '— Nikita B, Australia',
            description:
              'The resort excelled in all ways. The staff is super friendly &amp;amp; helpful, the food is amazing (specially their Al carte breakfast), the room and infinity pool has fantastic views overlooking the rice paddy fields and the jungle.',
            id: 'e19d53e1-999c-4703-8aef-7265f886531d',
          },
          {
            title: '— Michael S, Canada',
            description:
              'I loved Jannata , i loved the people providing the service there, Always smiling always nice, they are so friendly that i really missed them during the rest of my trip and they made it harder for the other hotel staff to beat their friendly nice service.',
            id: 'e19d53e1-999c-4703-8aef-7265f886531d',
          },
          {
            title: '— Laurenbull29, Germany',
            description:
              'We could not thank all the staff at Jannata Resort and Spa enough! We stayed for 3 night at the end of October for our Honeymoon. We was upgraded to a pool villa for our stay and treated like royalty, Our private infinity pool was so beautiful and the views from our villa were breath taking!',
            id: 'e19d53e1-999c-4703-8aef-7265f886531d',
          },
          {
            title: '— Laurenbull29, Germany',
            description:
              'We could not thank all the staff at Jannata Resort and Spa enough! We stayed for 3 night at the end of October for our Honeymoon. We was upgraded to a pool villa for our stay and treated like royalty, Our private infinity pool was so beautiful and the views from our villa were breath taking!',
            id: 'e19d53e1-999c-4703-8aef-7265f886531d',
          },
        ],
      },
    }
  },
  created() {
    const that = this
    this.$nextTick(() => {
      that.swipper = new Swiper('.mySwiper', {
        slidesPerView: 1,
        spaceBetween: 30,
        loop: true,
        centeredSlides: true,
        autoplay: {
          delay: 1000,
          disableOnInteraction: false,
        },
        pagination: {
          el: '.swiper-pagination',
          clickable: true,
        },
        navigation: {
          nextEl: '.swiper-button-next',
          prevEl: '.swiper-button-prev',
        },
      })
    })
  },
}
</script>

<style lang="scss" scoped>
#testiTwo {
  position: relative;
}

.flickity-enabled.is-draggable .flickity-viewport {
  cursor: move;
  cursor: -webkit-grab;
  cursor: grab;
}

.flickity-viewport {
  overflow: hidden;
  position: relative;
  height: 100%;
}

.flickity-slider {
  position: absolute;
  width: 100%;
  height: 100%;
}

.testi .slide {
  width: 100%;
  padding-bottom: 50px;
}

#page_summary .type-1 p {
  text-align: center;
  margin: 0;
  font-size: 20px;
}

#page_summary .type-1 p {
  font-family: Playfair Display, serif;
}

#page_summary .type-1 small {
  display: block;
  font-size: 15px;
  margin-top: 30px;
}

.flickity-page-dots {
  position: absolute;
  width: 100%;
  bottom: -25px;
  padding: 0;
  margin: 0;
  list-style: none;
  text-align: center;
  line-height: 1;
}

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
}

.swiper-slide img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
