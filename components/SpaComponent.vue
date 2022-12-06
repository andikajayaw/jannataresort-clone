<template>
  <div>
    <div
      data-scroll
      data-scroll-speed="-2"
      class="bg-image is-inview"
      :style="{
        backgroundImage: [
          `url(${model.featured.aws_file_url}/${model.featured.path}/${model.featured.filename.big})`,
        ],
      }"
      style="
        transform: matrix3d(1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
      "
    ></div>
    <div class="q-container container-inner">
      <div class="columns overlap-wrapper type-1">
        <div class="column block-entry">
          <div class="inner">
            <h2
              class="title rev_item"
              style="opacity: 1; transform: matrix(1, 0, 0, 1, 0, 0)"
            >
              RELAXING WITH JANNATA.
            </h2>
            <div class="title-line"></div>
            <p
              class="rev_item"
              style="opacity: 1; transform: matrix(1, 0, 0, 1, 0, 0)"
            >
              A sanctuary for the senses, Champaka Spa features a comfortable
              lounge area and three private treatment rooms for sessions of
              personal rejuvenation. This charming wellness facility overlooks a
              tropical valley that descends down to flowing river.
            </p>
            <br />
            <div
              class="rev_item"
              style="opacity: 1; transform: matrix(1, 0, 0, 1, 0, 0)"
            >
              <a
                class="inline-link q_magnet"
                style="transform: translate(0px, 0px)"
                >Read More</a
              >
            </div>
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
      name: 'Component Five',
      component_name: 'ComponentFive',

      model: {
        title: 'RELAXING WITH JANNATA.',
        description:
          'A sanctuary for the senses, Champaka Spa features a comfortable lounge area and three private treatment rooms for sessions of personal rejuvenation. This charming wellness facility overlooks a tropical valley that descends down to flowing river.',
        featured: {
          id: '5e6f379e9dae8c6e6bb078fc',
          created_at: '2020-03-16 08:23:58',
          updated_at: '2020-03-16 08:23:58',
          updatedBy: null,
          title: null,
          description: null,
          size: 79004,
          type: 'IMG',
          original: '6fe77037-cba3-4b76-81d0-bac03e031898.jpg',
          path: '5e65fe109dae8c14dd70f7e0/pictures/homepage/15843470372741',
          is_aws: true,
          aws_file_url:
            'https://vold-chain-hotel.s3-ap-southeast-1.amazonaws.com',
          filename: {
            big: 'big/6fe77037-cba3-4b76-81d0-bac03e031898.jpg',
            raw: 'raw/6fe77037-cba3-4b76-81d0-bac03e031898.jpg',
            blur: 'blur/6fe77037-cba3-4b76-81d0-bac03e031898.jpg',
            medium: 'medium/6fe77037-cba3-4b76-81d0-bac03e031898.jpg',
          },
        },
        link: {
          title: 'Read More',
          url: 'champaka-spa',
        },
      },
    }
  },
}
</script>

<style lang="scss" scoped>
.bg-full-image .bg-image {
  -o-object-fit: cover;
  object-fit: cover;
  width: 100%;
  height: 130%;
  position: absolute;
  top: 0;
  left: 0;
  z-index: 0;
  opacity: 0.5;
  background: no-repeat 50%;
  background-size: cover;
}

.bg-full-image * {
  color: #fff;
}
</style>
