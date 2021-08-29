<template>
  <div class="container">
    <div class="card">
      <div class="flex w-full">
        <div class="w-40 mx-2">
          <product-carousel
            :items="imageLists"
          ></product-carousel>
        </div>
        <div class="w-60 mx-2">
          <h1>Macbook Pro</h1>
          <small>4.3 (dari 10 ulasan) | 15 terjual</small>
          <h1 class="text-red">Rp. 999,000</h1>
          <hr />
          <small>Pengiriman</small>
          <div></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ProductCarousel from '../components/ProductCarousel.vue';

export default {
  name: 'Home',
  components: {
    ProductCarousel,
  },
  data() {
    return {
      imageLists: [
        {
          src: 'https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Vue.js_Logo_2.svg/2367px-Vue.js_Logo_2.svg.png',
          alt: 'Vue Logo',
        },
        {
          src: 'https://upload.wikimedia.org/wikipedia/commons/thumb/2/29/Vue_International_Logo.jpg/1200px-Vue_International_Logo.jpg',
          alt: 'Vue Logo',
        },
        {
          src: 'https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Vue.js_Logo_2.svg/2367px-Vue.js_Logo_2.svg.png',
          alt: 'Vue Logo',
        },
        {
          src: 'https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Vue.js_Logo_2.svg/2367px-Vue.js_Logo_2.svg.png',
          alt: 'Vue Logo',
        },
        {
          src: 'https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Vue.js_Logo_2.svg/2367px-Vue.js_Logo_2.svg.png',
          alt: 'Vue Logo',
        },
      ],
    };
  },
};
</script>