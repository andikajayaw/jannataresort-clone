<template>
  <div class="q-container container-inner">
    <div class="columns">
      <div class="column">&nbsp;</div>
      <div class="column is-7">
        <h1
          class="section-headline rev_item"
          style="opacity: 1; transform: matrix(1, 0, 0, 1, 0, 0)"
        >
          THE STAY
        </h1>
        <div
          class="rev_item"
          style="opacity: 1; transform: matrix(1, 0, 0, 1, 0, 0)"
        >
          <p>
            Stylish accommodation option at Jannata Resort &amp; Spa
            incorporates a choice of 16 Deluxe Suites, 2 Deluxe Family Suite and
            2 Pool Villas to anticipate all of your holiday needs. All
            categories are the epitome of Balinese luxury with customized
            interiors and essential home comforts.
          </p>
          <p><br /></p>
          <p>
            During pandemic, our resort has applied health protocols to ensure
            that our guests are safe. Before check-in, guests are encouraged to
            wash their hands and our team will check guests' body temperature.
          </p>
          <p><br /></p>
          <p>
            All the team members of Jannata Resort maintain the cleanliness in
            all areas including hotel rooms, restaurant, spa, kitchen. Every 4
            hours disinfectant spray and physical distancing towards our pool
            decks, restaurant chairs, spa outlets are applied to ensure that our
            resort is in hygiene circumstance.
          </p>
          <p><br /></p>
          <p>
            Masks, face shields, hand sanitizer and also washing hands counter
            are fully prepared to welcome the new normal era ensuring all guests
            and staffs are safe and healthy.<br />
          </p>
          <p><br /></p>
        </div>
      </div>
    </div>
    <div class="columns">
      <div class="column villas-container">
        <div id="accommodations" class="accommodations column-grid-container">
          <!-- model.dataSlider.featured.aws_file_url + model.dataSlider.featured.path + model.dataSlider.featured.filename.big -->
          <div
            v-for="slider in model.dataSlider"
            :key="slider.id"
            class="accommodation-type column-item"
          >
            <!---->
            <br />
            <!---->
            <a
              ><h4 class="accommodation-name">{{ slider.link.title }}</h4>
              <div
                class="accommodation-bg"
                :style="{
                  backgroundImage: [
                    `url(${slider.featured.aws_file_url}/${slider.featured.path}/${slider.featured.filename.big})`,
                  ],
                }"
              ></div
            ></a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      name: 'Component Three',
      component_name: 'ComponentThree',
      model: {
        title: 'THE STAY',
        description:
          "<p>Stylish accommodation option at Jannata Resort &amp; Spa incorporates a choice of 16 Deluxe Suites, 2 Deluxe Family Suite and 2 Pool Villas to anticipate all of your holiday needs. All categories are the epitome of Balinese luxury with customized interiors and essential home comforts.</p><p><br></p><p>During pandemic, our resort has applied health protocols to ensure that our guests are safe. Before check-in, guests are encouraged to wash their hands and our team will check guests' body temperature.</p><p><br></p><p>All the team members of Jannata Resort maintain the cleanliness in all areas including hotel rooms, restaurant, spa, kitchen. Every 4 hours disinfectant spray and physical distancing towards our pool decks, restaurant chairs, spa outlets are applied to ensure that our resort is in hygiene circumstance.</p><p><br></p><p>Masks, face shields, hand sanitizer and also washing hands counter are fully prepared to welcome the new normal era ensuring all guests and staffs are safe and healthy.<br></p><p><br></p>",
        dataSlider: [
          {
            title: 'Slider Title',
            link: {
              title: 'Deluxe Suite',
              url: 'https://jannataresort.com/en/accommodation/deluxe-suite',
            },
            featured: {
              id: '5fa4f6979dae8c603924cc4d',
              created_at: '2020-11-06 07:09:11',
              updated_at: '2020-11-06 07:09:11',
              title: null,
              description: null,
              size: 271951,
              type: 'IMG',
              original: 'deluxes-suite_home1.jpg',
              path: '5e65fe109dae8c14dd70f7e0/pictures/3-img-homepage/16046465505451',
              is_aws: true,
              aws_file_url:
                'https://vold-chain-hotel.s3-ap-southeast-1.amazonaws.com',
              filename: {
                big: 'big/deluxes-suite_home1.jpg',
                raw: 'raw/deluxes-suite_home1.jpg',
                blur: 'blur/deluxes-suite_home1.jpg',
                medium: 'medium/deluxes-suite_home1.jpg',
              },
            },
            featured_hover: {
              id: '5fa51c299dae8c603924cc7b',
              created_at: '2020-11-06 09:49:29',
              updated_at: '2020-11-06 09:49:29',
              title: null,
              description: null,
              size: 279961,
              type: 'IMG',
              original: 'deluxes-suite_home3.jpg',
              path: '5e65fe109dae8c14dd70f7e0/pictures/3-img-homepage/16046561692221',
              is_aws: true,
              aws_file_url:
                'https://vold-chain-hotel.s3-ap-southeast-1.amazonaws.com',
              filename: {
                big: 'big/deluxes-suite_home3.jpg',
                raw: 'raw/deluxes-suite_home3.jpg',
                blur: 'blur/deluxes-suite_home3.jpg',
                medium: 'medium/deluxes-suite_home3.jpg',
              },
            },
            id: '4d4ea967-dca0-45ad-bb85-990632a9c6b5',
          },
          {
            title: 'Slider Title',
            link: {
              title: 'Superior Room',
              url: 'https://jannataresort.com/en/accommodation/deluxe-twin',
            },
            featured: {
              id: '5fa4f7989dae8c603924cc5c',
              created_at: '2020-11-06 07:13:28',
              updated_at: '2020-11-06 07:13:28',
              title: null,
              description: null,
              size: 312847,
              type: 'IMG',
              original: 'superior-room_home2.jpg',
              path: '5e65fe109dae8c14dd70f7e0/pictures/3-img-homepage/16046468078752',
              is_aws: true,
              aws_file_url:
                'https://vold-chain-hotel.s3-ap-southeast-1.amazonaws.com',
              filename: {
                big: 'big/superior-room_home2.jpg',
                raw: 'raw/superior-room_home2.jpg',
                blur: 'blur/superior-room_home2.jpg',
                medium: 'medium/superior-room_home2.jpg',
              },
            },
            featured_hover: {
              id: '5fa4f7979dae8c603924cc5b',
              created_at: '2020-11-06 07:13:27',
              updated_at: '2020-11-06 07:13:27',
              title: null,
              description: null,
              size: 268773,
              type: 'IMG',
              original: 'superior-room_home1.jpg',
              path: '5e65fe109dae8c14dd70f7e0/pictures/3-img-homepage/16046468070171',
              is_aws: true,
              aws_file_url:
                'https://vold-chain-hotel.s3-ap-southeast-1.amazonaws.com',
              filename: {
                big: 'big/superior-room_home1.jpg',
                raw: 'raw/superior-room_home1.jpg',
                blur: 'blur/superior-room_home1.jpg',
                medium: 'medium/superior-room_home1.jpg',
              },
            },
            id: '4d4ea967-dca0-45ad-bb85-990632a9c6b5',
          },
          {
            title: 'Slider Title',
            link: {
              title: 'Pool Villa',
              url: 'https://jannataresort.com/en/accommodation/pool-villa',
            },
            featured: {
              id: '5edf4cbd9dae8c54fa82ddfe',
              created_at: '2020-06-09 08:47:57',
              updated_at: '2020-06-09 08:47:57',
              title: null,
              description: null,
              size: 1760246,
              type: 'IMG',
              original: 'DJI_0593_JPG.jpg',
              path: '5e65fe109dae8c14dd70f7e0/pictures/accomodation/pool-villa/15916924764352',
              is_aws: true,
              aws_file_url:
                'https://vold-chain-hotel.s3-ap-southeast-1.amazonaws.com',
              filename: {
                big: 'big/DJI_0593_JPG.jpg',
                raw: 'raw/DJI_0593_JPG.jpg',
                blur: 'blur/DJI_0593_JPG.jpg',
                medium: 'medium/DJI_0593_JPG.jpg',
              },
            },
            featured_hover: {
              id: '5fa62cc69dae8c603924ccf2',
              created_at: '2020-11-07 05:12:38',
              updated_at: '2020-11-07 05:12:38',
              title: null,
              description: null,
              size: 287924,
              type: 'IMG',
              original: 'pool-villa_home2.jpg',
              path: '5e65fe109dae8c14dd70f7e0/pictures/3-img-homepage/16047259573881',
              is_aws: true,
              aws_file_url:
                'https://vold-chain-hotel.s3-ap-southeast-1.amazonaws.com',
              filename: {
                big: 'big/pool-villa_home2.jpg',
                raw: 'raw/pool-villa_home2.jpg',
                blur: 'blur/pool-villa_home2.jpg',
                medium: 'medium/pool-villa_home2.jpg',
              },
            },
            id: '4d4ea967-dca0-45ad-bb85-990632a9c6b5',
          },
        ],
      },
    }
  },
}
</script>

<style lang="scss" scoped></style>
