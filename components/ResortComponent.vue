<template>
  <div>
    <div style="background: red; width: 100%; height: 100%">
      <h1>
        {{ model.title }}
      </h1>
      <div>
        <img
          :src="`${model.featured.aws_file_url}/${model.featured.path}/${model.featured.filename.raw}`"
          alt="Resort"
        />
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

<style lang="scss" scoped></style>
