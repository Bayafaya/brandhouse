<template>
  <div class="stories">
    <span>Истории</span>
    <swiper :modules="modules" :slides-per-view="4.3" :space-between="12">
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
  components: { Swiper, SwiperSlide },
  setup() {
    return {
      modules: [Pagination, Autoplay, Scrollbar],
    };
  },
  props: {
    darkMode: {
      type: Boolean,
      required: true,
    },
  },
  watch: {
    darkMode(newValue) {
      if (newValue) {
        const current = document.getElementsByClassName("stories");
        current[0].classList.toggle("dark");
        const storyItems = document.getElementsByClassName("story__item");
          for (let index = 0; index < storyItems.length; index++) {
            const element = storyItems[index];
            element.classList.toggle("border__changed")
          }
      } else {
        const current = document.getElementsByClassName("stories");
        current[0].classList.toggle("dark");
        const storyItems = document.getElementsByClassName("story__item");
        for (let index = 0; index < storyItems.length; index++) {
            const element = storyItems[index];
            element.classList.toggle("border__changed")
          }
      }
    },
  },
};
</script>

<style scoped>
.stories {
  background: var(--secondary-light);
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
.stories span {
  display: block;
  font-family: "SF UI Display";
  font-style: normal;
  font-weight: 500;
  font-size: 22px;
  line-height: 28px;
  margin-bottom: 12px;
}
.dark {
  background: var(--black);
}
.border__changed {
  border: 2px solid rgba(120, 120, 128, 0.3);
}
</style>
