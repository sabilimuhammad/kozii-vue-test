<template>
  <div>
    <div class="product-main-image">
      <img
        :src="activeImage.src"
        :alt="activeImage.alt"
      >
    </div>
    <div class="flex w-full">
      <div
        v-for="(img, i) in items"
        :key="`image-${i}`"
        class="w-25 mx-2 pointer"
        :class="activeIndex === i && 'product--active'"
      >
        <img
          :src="img.src"
          :alt="img.alt"
          @click="setActiveImage(img, i)"
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    items: {
      type: Array,
      default: () => [],
      required: true,
    },
  },
  data() {
    return {
      activeImage: {
        src: '',
        alt: '',
      },
      activeIndex: 0,
    };
  },
  mounted() {
    // eslint-disable-next-line prefer-destructuring
    this.activeImage = this.items[0];
  },
  methods: {
    setActiveImage(img, index) {
      this.activeImage = img;
      this.activeIndex = index;
    },
  },
};
</script>