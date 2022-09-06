<template>
      <div class="stories">
      <h2>Истории</h2>
      <swiper
        :modules="modules"
        :slides-per-view="4.3"
        :space-between="12"
        @swiper="onSwiper"
        @slideChange="onSlideChange"
      >
        <swiper-slide>
          <div class="story__item">
            <img class="story__img" src="../image/1.png" alt="story" /></div
        ></swiper-slide>
        <swiper-slide>
          <div class="story__item">
            <img class="story__img" src="../image/2.png" alt="story" /></div
        ></swiper-slide>
        <swiper-slide>
          <div class="story__item">
            <img class="story__img" src="../image/3.png" alt="story" /></div
        ></swiper-slide>
        <swiper-slide>
          <div class="story__item">
            <img class="story__img" src="../image/4.png" alt="story" /></div
        ></swiper-slide>
        <swiper-slide>
          <div class="story__item">
            <img class="story__img" src="../image/1.png" alt="story" /></div
        ></swiper-slide>
        <swiper-slide>
          <div class="story__item">
            <img class="story__img" src="../image/2.png" alt="story" /></div
        ></swiper-slide>
        <swiper-slide>
          <div class="story__item">
            <img class="story__img" src="../image/3.png" alt="story" /></div
        ></swiper-slide>
        <swiper-slide>
          <div class="story__item">
            <img class="story__img" src="../image/4.png" alt="story" /></div
        ></swiper-slide>
      </swiper>
    </div>
</template>

<script>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Pagination, Autoplay, Scrollbar } from "swiper";
import "swiper/css";
export default {
    components: {Swiper, SwiperSlide},
  setup() {
    return {
      modules: [Pagination, Autoplay, Scrollbar],
    };
  },
}
</script>

<style scoped>
.stories {
  background: #f2f2f7;
  padding: 16px 16px 32px 16px;
}
.story__item {
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 4px;
  width: 76px;
  height: 92px;
  border: 2px solid rgba(120, 120, 128, 0.16);
}
.story__img {
  border-radius: 3px;
  padding: 2px;
  width: 72px;
  height: 88px;
}
</style>