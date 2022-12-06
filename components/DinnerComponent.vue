<template>
  <div class="q-container container-inner">
    <div class="columns overlap-wrapper type-1">
      <div class="column block-picture wide">
        <figure class="picture">
          <div class="rev_clip" style="clip-path: inset(0px); opacity: 1">
            <img
              :src="`${model.featured.aws_file_url}/${model.featured.path}/${model.featured.filename.big}`"
              alt=""
              data-scroll
              data-scroll-speed="-2"
              class="clip_image is-inview"
            />
          </div>
        </figure>
      </div>
      <div
        class="column block-entry bg-white div-transform"
        data-scroll
        data-scroll-speed="-2"
      >
        <div class="inner">
          <h2 class="title">
            <span class="q_split"
              ><span
                class="q_split_wrap rev_item"
                style="opacity: 1; transform: matrix(1, 0, 0, 1, 0, 0)"
                >DINNER WITH</span
              ></span
            >
            <span class="q_split text-green"
              ><span
                class="q_split_wrap rev_item"
                style="opacity: 1; transform: matrix(1, 0, 0, 1, 0, 0)"
                >JANNATA</span
              ></span
            >
          </h2>
          <div class="title-line"></div>
          <div>
            <p>
              Amateras Restaurant at Jannata Resort &amp; Spa serves an
              extensive menu of Western and Asian cuisine that is driven by
              quality ingredients.
            </p>
            <p><br /></p>
            <p>
              The restaurant is located next to the lobby and extends out onto
              an open terrace for an alfresco dining experience. It is elevated
              over the main swimming pool with tropical views of lush valley
              greenery in the distance.
            </p>
          </div>
          <div
            class="rev_item"
            style="opacity: 1; transform: matrix(1, 0, 0, 1, 0, 0)"
          >
            <a class="inline-link q_magnet"> Read More </a>
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
      name: 'Component Four',
      component_name: 'ComponentFour',
      model: {
        featured: {
          id: '5e78388d9dae8c62826241d8',
          created_at: '2020-03-23 04:18:21',
          updated_at: '2020-03-23 04:18:21',
          updatedBy: null,
          title: null,
          description: null,
          size: 195994,
          type: 'IMG',
          original: 'e061b86c-217c-4b9f-87ec-bc67b45db7a0.jpg',
          path: '5e65fe109dae8c14dd70f7e0/pictures/dining/15849371005791',
          is_aws: true,
          aws_file_url:
            'https://vold-chain-hotel.s3-ap-southeast-1.amazonaws.com',
          filename: {
            big: 'big/e061b86c-217c-4b9f-87ec-bc67b45db7a0.jpg',
            raw: 'raw/e061b86c-217c-4b9f-87ec-bc67b45db7a0.jpg',
            blur: 'blur/e061b86c-217c-4b9f-87ec-bc67b45db7a0.jpg',
            medium: 'medium/e061b86c-217c-4b9f-87ec-bc67b45db7a0.jpg',
          },
        },
        title_one: 'DINNER WITH',
        title_two: 'JANNATA',
        description:
          '<p>Amateras Restaurant at Jannata Resort &amp; Spa serves an extensive menu of Western and Asian cuisine that is driven by quality ingredients.</p><p><br></p><p>The restaurant is located next to the lobby and extends out onto an open terrace for an alfresco dining experience. It is elevated over the main swimming pool with tropical views of lush valley greenery in the distance.</p>',
        link: {
          title: 'Read More',
          url: 'amateras-dining',
        },
      },
    }
  },
}
</script>

<style lang="scss" scoped>
.clip_image {
  height: 641.3px !important;
  width: auto !important;
  transform: matrix3d(1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
}
.picture {
  height: 583px !important;
}

.rev_clip {
  clip-path: inset(0 1000px 0 0);
  -webkit-clip-path: inset(0 1000px 0 0);
  height: 100%;
  position: relative;
  z-index: 5;
  min-height: 250px;
}

.rev_clip img[data-v-5004e6cc] {
  position: absolute;
  max-width: 200%;
  width: 100%;
  min-width: 100%;
  min-height: 250px;
}

.div-transform {
  transform: matrix3d(1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);
}

.block-card-overlap .type-1 .block-entry {
  right: 0;
  left: -300px;
}

@media screen and (max-width: 540px) {
  .picture {
    height: 298px !important;
  }
  .clip_image {
    height: 450px !important;
    width: auto !important;
  }
  .block-card-overlap .block-picture .picture {
    padding: 0 20px 0 0;
  }
}

@media screen and (min-width: 768px) {
  .clip_image {
    height: 641.3px !important;
    width: auto !important;
  }
  .picture {
    height: 583px !important;
  }
}
</style>
