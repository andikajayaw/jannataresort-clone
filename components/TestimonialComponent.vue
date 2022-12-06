<template>
  <div class="swiper mySwiper">
    <div class="swiper-wrapper">
      <div
        v-for="slider in model.dataSlider"
        :key="slider.id"
        class="slide swiper-slide"
        aria-hidden="true"
      >
        <div>
          <p>
            {{ slider.description }}
          </p>
        </div>
        <br />
        <br />
        <br />
        <!-- <div>
          <span>{{ slider.title }}</span>
        </div> -->
      </div>
    </div>
    <!-- <div class="swiper-button-next"></div>
      <div class="swiper-button-prev"></div> -->
    <div class="swiper-pagination"></div>
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
      })
    })
  },
}
</script>

<style lang="scss" scoped>
.slide {
  width: 100%;
  padding-bottom: 50px;
}

p {
  font-family: Playfair Display, serif;
  text-align: center;
  margin: 0;
  font-size: 20px;
}

small {
  display: block;
  font-size: 15px;
  margin-top: 30px;
}

.swiper {
  width: 100%;
  height: 100%;
}

.swiper-slide {
  text-align: center;
  font-size: 18px;

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
