<template>
  <div style="width: 100%; max-width: 800px; margin: 20px auto">
    <h1>Second Demo - Vue Awesome Swiper</h1>
    <swiper class="swiper" :options="swiperOption">
      <swiper-slide>
        <img
          src="https://res.cloudinary.com/dpkreativ/image/upload/v1646483551/wallpapers/car.jpg"
          alt="car"
        />
      </swiper-slide>
      <swiper-slide>
        <img
          src="https://res.cloudinary.com/dpkreativ/image/upload/v1646695756/wallpapers/laptop.jpg"
          alt="laptop"
        />
      </swiper-slide>
      <swiper-slide>
        <img
          src="https://res.cloudinary.com/dpkreativ/image/upload/v1646749176/wallpapers/photo-1646727002357-073c182015e0_qv2xlg.jpg"
          alt="mist"
        />
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
      <div class="swiper-button-prev" slot="button-prev"></div>
      <div class="swiper-button-next" slot="button-next"></div>
    </swiper>
  </div>
</template>

<script>
import { Swiper, SwiperSlide, directive } from 'vue-awesome-swiper'

export default {
  name: 'SecondDemo',
  components: {
    Swiper,
    SwiperSlide,
  },
  directives: {
    swiper: directive,
  },
  data() {
    return {
      swiperOption: {
        slidesPerView: 1,
        spaceBetween: 20,
        loop: true,
        pagination: {
          el: '.swiper-pagination',
          clickable: true,
        },
        navigation: {
          nextEl: '.swiper-button-next',
          prevEl: '.swiper-button-prev',
        },
      },
    }
  },
}
</script>
