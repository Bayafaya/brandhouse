<template>
  <div class="slider">
    <div class="banner__scroll">
      <swiper
        :modules="modules"
        :slides-per-view="1"
        :space-between="0"
        :pagination="{ clickable: true }"
        :autoplay="{ delay: 2000, disableOnInteraction: false }"
        @swiper="onSwiper"
        @slideChange="onSlideChange"
      >
        <swiper-slide
          ><img
            class="slider__banner"
            src="../image/b24ea1edbecbac9_750x485.jpg"
            alt="slider__banner"
        /></swiper-slide>
        <swiper-slide
          ><img
            class="slider__banner"
            src="../image/46230116.jpg"
            alt="slider__banner"
        /></swiper-slide>
        <swiper-slide
          ><img
            class="slider__banner"
            src="../image/03893925.jpg"
            alt="slider__banner"
        /></swiper-slide>
      </swiper>
    </div>
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Pagination, Autoplay} from "swiper";
import "swiper/css";
import "swiper/css/pagination";
import "swiper/css/autoplay";

export default {
  components: { Swiper, SwiperSlide },
  setup() {
    return {
      modules: [Pagination, Autoplay],
    };
  },
};
</script>

<style scoped>
.slider {
  padding: 24px 16px 16px;
}
.slider__banner {
  height: 200px;
  width: 100%;
  border-radius: 4px;
}
.banner__scroll {
  margin: 0 auto;
}
</style>
