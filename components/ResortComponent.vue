<template>
  <div class="q-container container-inner">
    <div class="columns block-card-shadow">
      <div class="column is-7 block-picture">
        <figure class="picture" style="height: 650px">
          <div
            data-scroll=""
            data-scroll-speed="-1"
            class="box wide is-inview"
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
                -23.06,
                0,
                1
              );
            "
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
.bg-vanilla {
  background-color: #f0f0f5;
}

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

.block-card-shadow .block-picture .picture {
  position: relative;
  margin: 0;
  padding: 0 30px 0 20px;
  height: 100%;
}

.block-card-shadow .block-picture .box.wide {
  position: absolute;
  top: 60px;
  right: -80%;
  width: 140%;
}

.block-card-shadow .block-picture .box {
  position: absolute;
  top: 60px;
  right: 0;
  width: 83%;
  height: 100%;
  background-color: #d8d6e2;
  z-index: 0;
}

.block-card-shadow .block-picture .picture .rev_clip {
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

.block-card-shadow .block-entry {
  display: flex;
  justify-content: flex-end;
  -webkit-justify-content: flex-end;
  align-items: center;
  -webkit-align-items: center;
  flex: none;
  width: 42.5%;
}

.block-card-shadow .block-entry .inner {
  padding: 0 50px 0 100px;
}

.block-card-shadow .block-entry .section-headline {
  margin-top: 100px;
}
.section-headline {
  font: 400 35px/1.3 Playfair Display, serif;
  text-transform: uppercase;
  letter-spacing: 5px;
  color: #5f5c68;
  position: relative;
  margin-top: 0;
  display: block;
  margin-bottom: 50px;
}

.q_split {
  display: block;
  overflow: hidden;
}

.inline-link {
  padding: 20px;
  margin-left: -20px;
  position: relative;
  display: inline-block;
  font-size: 10px;
  text-transform: uppercase;
  letter-spacing: 1px;
}

.inline-link.q_magnet {
  display: inline-block;
}

.inline-link::before {
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

.inline-link:hover:before {
  width: 100%;
  width: calc(100% - 40px);
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
