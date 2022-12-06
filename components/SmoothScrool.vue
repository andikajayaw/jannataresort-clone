<template>
  <div data-scroll-container>
    <slot></slot>
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      scroll: null,
    }
  },
  mounted() {
    const that = this
    this.$nextTick(() => {
      that.scroll = new that.LocomotiveScroll({
        el: document.querySelector('[data-scroll-container]'),
        smooth: true,
      })
    })
  },
}
</script>
