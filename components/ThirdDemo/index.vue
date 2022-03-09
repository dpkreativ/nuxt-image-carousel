<template>
  <div style="width: 100%; max-width: 800px; margin: 20px auto">
    <h1>Third Demo - Vue Slick Carousel</h1>
    <!-- Implementation -->
    <div>
      <VueSlickCarousel v-bind="slickOptions">
        <div>
          <img
            src="https://res.cloudinary.com/dpkreativ/image/upload/v1646483551/wallpapers/car.jpg"
            alt="car"
          />
        </div>
        <div>
          <img
            src="https://res.cloudinary.com/dpkreativ/image/upload/v1646695756/wallpapers/laptop.jpg"
            alt="laptop"
          />
        </div>
        <div>
          <img
            src="https://res.cloudinary.com/dpkreativ/image/upload/v1646749176/wallpapers/photo-1646727002357-073c182015e0_qv2xlg.jpg"
            alt="mist"
          />
        </div>
      </VueSlickCarousel>
    </div>
  </div>
</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
export default {
  name: 'ThirdDemo',
  components: {
    VueSlickCarousel,
  },
  data() {
    return {
      slickOptions: {
        slidesToShow: 1,
      },
    }
  },
}
</script>

<style>
.slick-next:before,
.slick-prev:before {
  color: black;
}
</style>
