<template>
  <div class="q-container container-inner">
    <div class="columns block-card-shadow">
      <div class="column is-7 block-picture">
        <figure class="picture">
          <div
            data-scroll=""
            data-scroll-speed="-1"
            class="box wide is-inview"
          ></div>
          <div
            class="rev_clip"
            style="clip-path: inset(0px); transform: matrix(1, 0, 0, 1, -50, 0)"
          >
            <img
              :src="`${model.featured.aws_file_url}/${model.featured.path}/${model.featured.filename.big}`"
              alt=""
              data-scroll=""
              data-scroll-speed="-0.95"
              class="clip_image is-inview"
            />
          </div>
        </figure>
      </div>
      <div class="column is-5 block-entry">
        <div class="inner">
          <h1
            class="section-headline rev_item"
            style="transform: matrix(1, 0, 0, 1, 0, 0)"
          >
            <span class="q_split">THE&nbsp;<br />RESORT</span>
          </h1>
          <div
            class="rev_item"
            style="opacity: 1; transform: matrix(1, 0, 0, 1, 0, 0)"
          >
            Jannata Resort &amp; Spa is a boutique property with tranquil valley
            views in the rural village of Sebali, just outside of Ubud.<br /><br />It
            is attuned to the surrounding environment through a thoughtful
            design that respects Bali’s rich artistry and cultural heritage.
          </div>
          <div
            class="rev_item"
            style="opacity: 1; transform: matrix(1, 0, 0, 1, 0, 0)"
          >
            <a href="/en/our-story" class="inline-link q_magnet"
              >READ THE STORY</a
            >
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
      name: 'Component Two',
      component_name: 'ComponentTwo',
      model: {
        title: 'THE <br>RESORT',
        description:
          'Jannata Resort & Spa is a boutique property with tranquil valley views in the rural village of Sebali, just outside of Ubud.<br><br>It is attuned to the surrounding environment through a thoughtful design that respects Bali’s rich artistry and cultural heritage.',
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
        link: {
          title: 'READ THE STORY',
          url: 'our-story',
        },
      },
    }
  },
}
</script>

<style lang="scss" scoped>
.clip_image {
  height: 715px !important;
  width: auto !important;
}
.picture {
  height: 650px !important;
}
.rev_clip img {
  position: absolute;
  max-width: 200%;
  width: 100%;
  min-width: 100%;
  min-height: 250px;
}
@media screen and (max-width: 768px) {
  .block-card-shadow {
    display: flex;
  }

  .picture {
    height: 417px !important;
  }

  .clip_image {
    height: 458.7px !important;
    width: auto !important;
  }
}

@media screen and (min-width: 768px) {
  .block-card-shadow .block-entry .inner {
    padding-left: 0;
  }
}

@media screen and (max-width: 540px) {
  .picture {
    height: 599px !important;
  }
  .clip_image {
    height: 458.7px !important;
    width: auto !important;
    left: 50px;
  }
}
</style>
