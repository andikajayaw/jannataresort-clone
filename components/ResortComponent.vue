<template>
  <div>
    <div class="container-inner">
      <div class="columns block-card-shadow">
        <div class="column is-7 block-picture">
          <figure class="picture">
            <div class="box wide"></div>
            <div
              class="rev_clip"
              data-v-3c5fc44e=""
              style="
                clip-path: inset(0px);
                opacity: 0;
                transform: matrix(1, 0, 0, 1, -50, 0);
              "
            >
              <img
                :src="`${model.featured.aws_file_url}/${model.featured.path}/${model.featured.filename.big}`"
                alt=""
                data-scroll=""
                data-scroll-speed="-0.95"
                class="clip_image is-inview"
                style="
                  transform: matrix3d(
                    1,
                    0,
                    0,
                    0,
                    0,
                    1,
                    0,
                    0,
                    0,
                    0,
                    1,
                    0,
                    0,
                    0,
                    0,
                    1
                  );
                  height: 715px;
                  width: auto;
                "
              />
            </div>
          </figure>
        </div>
        <div class="column is-5 block-entry">
          <div class="inner">
            <h1
              class="section-headline rev_item"
              style="opacity: 0; transform: matrix(1, 0, 0, 1, 0, 0)"
            >
              <span class="q_split">THE&nbsp;<br />RESORT</span>
            </h1>
            <div
              class="rev_item"
              style="opacity: 1; transform: matrix(1, 0, 0, 1, 0, 0)"
            >
              Jannata Resort &amp; Spa is a boutique property with tranquil
              valley views in the rural village of Sebali, just outside of
              Ubud.<br /><br />It is attuned to the surrounding environment
              through a thoughtful design that respects Bali’s rich artistry and
              cultural heritage.
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
      <h1>
        {{ model.title }}
      </h1>
      <div>
        <img alt="Resort" />
        <!-- {{ model.description }} -->
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
.container-inner {
  padding-left: 12rem;
  padding-right: 12rem;
}

.block-card-shadow {
  padding: 50px 0 80px;
}

.block-card-shadow .block-picture {
  flex: none;
  width: 57.5%;
}

.picture {
  position: relative;
  margin: 0;
  padding: 0 30px 0 20px;
  height: 100%;
}

.box.wide {
  position: absolute;
  top: 60px;
  right: -80%;
  width: 140%;
}

.rev_clip {
  height: 100%;
  position: relative;
  z-index: 5;
}

.rev_clip img {
  position: absolute;
  max-width: 200%;
  width: 100%;
  min-width: 100%;
  min-height: 250px;
}

.block-entry {
  display: flex;
  justify-content: flex-end;
  -webkit-justify-content: flex-end;
  align-items: center;
  -webkit-align-items: center;
  flex: none;
  width: 42.5%;
}

.inner {
  padding: 0 50px 0 100px;
}

.section-headline {
  margin-top: 100px;
}

.q_split,
.q_split_wrap {
  display: block;
}

.q_split {
  overflow: hidden;
}

.inline-link.q_magnet {
  display: inline-block;
}

.inline-link:before {
  content: '';
  display: block;
  position: absolute;
  bottom: 0;
  left: 20px;
  width: 0;
  height: 2px;
  background: #679334;
  transition: all 0.5s cubic-bezier(0.86, 0, 0.07, 1);
}
</style>
