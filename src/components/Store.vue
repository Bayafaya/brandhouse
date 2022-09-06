<template>
  <div class="store">
    <div class="header__of__products">
      <span>Топ магазины</span>
      <button class="all_products">все магазины</button>
    </div>
    <div class="store__card">
      <swiper
        :modules="modules"
        :slides-per-view="1.05"
        :space-between="8"
        @swiper="onSwiper"
        @slideChange="onSlideChange"
      >
        <swiper-slide>
          <div class="store__item">
            <img src="../image/top store.png" alt="store" />
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="store__item">
            <img src="../image/top store.png" alt="store" />
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="store__item">
            <img src="../image/top store.png" alt="store" />
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
    components: {Swiper, SwiperSlide},
}
</script>

<style scoped>
.store {
  padding: 0px 16px 24px 16px;
}
.store__item img {
  height: 160px;
  width: 100%;
  border-radius: 4px;
}
.store__card {
  padding: 24px 0;
}
</style>
