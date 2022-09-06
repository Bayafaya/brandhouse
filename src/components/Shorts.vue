<template>
      <div class="shorts">
      <div class="header__of__products">
        <span>Видео обзоры</span>
        <button class="all_products">все видео</button>
      </div>
      <div class="shorts__bar">
        <swiper
          :modules="modules"
          :slides-per-view="2.1"
          :space-between="8"
          @swiper="onSwiper"
          @slideChange="onSlideChange"
        >
          <swiper-slide>
            <div class="shorts__item">
              <img src="../image/Video.png" alt="Video" />
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="shorts__item">
              <img src="../image/Video 2.png" alt="Video" />
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="shorts__item">
              <img src="../image/Video.png" alt="Video" />
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="shorts__item">
              <img src="../image/Video 2.png" alt="Video" />
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="shorts__item">
              <img src="../image/Video.png" alt="Video" />
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="shorts__item">
              <img src="../image/Video 2.png" alt="Video" />
            </div>
          </swiper-slide>
        </swiper>
      </div>
    </div>
</template>

<script>
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";

export default {
  components: { Swiper, SwiperSlide },
};
</script>

<style scoped>
.shorts{
  padding: 24px 16px;
}
.shorts__bar{
  padding: 24px 0;
}
.shorts__item img{
  height: 220px;
  width: 100%;
  border-radius: 4px;
}
</style>