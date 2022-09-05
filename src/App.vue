<template>
  <div>
    <div class="search__area">
      <div class="search__input">
        <img src="./image/ri-search-2-line.svg" alt="search" />
        <my-input type="text" placeholder="Поиск товара" />
      </div>
    </div>
    <div class="stories">
      <h2>Истории</h2>
      <swiper
        :slides-per-view="4.3"
        :space-between="12"
        @swiper="onSwiper"
        @slideChange="onSlideChange"
      >
        <swiper-slide>
          <div class="story__item">
            <img class="story__img" src="./image/1.png" alt="story" /></div
        ></swiper-slide>
        <swiper-slide>
          <div class="story__item">
            <img class="story__img" src="./image/2.png" alt="story" /></div
        ></swiper-slide>
        <swiper-slide>
          <div class="story__item">
            <img class="story__img" src="./image/3.png" alt="story" /></div
        ></swiper-slide>
        <swiper-slide>
          <div class="story__item">
            <img class="story__img" src="./image/4.png" alt="story" /></div
        ></swiper-slide>
        <swiper-slide>
          <div class="story__item">
            <img class="story__img" src="./image/1.png" alt="story" /></div
        ></swiper-slide>
        <swiper-slide>
          <div class="story__item">
            <img class="story__img" src="./image/2.png" alt="story" /></div
        ></swiper-slide>
        <swiper-slide>
          <div class="story__item">
            <img class="story__img" src="./image/3.png" alt="story" /></div
        ></swiper-slide>
        <swiper-slide>
          <div class="story__item">
            <img class="story__img" src="./image/4.png" alt="story" /></div
        ></swiper-slide>
      </swiper>
    </div>
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
              class="slider__baner"
              src="./image/b24ea1edbecbac9_750x485.jpg"
              alt=""
          /></swiper-slide>
          <swiper-slide
            ><img class="slider__baner" src="./image/46230116.jpg" alt=""
          /></swiper-slide>
          <swiper-slide
            ><img class="slider__baner" src="./image/03893925.jpg" alt=""
          /></swiper-slide>
          ...
        </swiper>
      </div>
    </div>
    <div class="banners">
      <div class="banners__content">
        <img class="banner_item" src="./image/banner1.png" alt="banners" />
        <img class="banner_item" src="./image/banner2.png" alt="banners" />
        <img class="banner_item" src="./image/banner3.png" alt="banners" />
      </div>
    </div>
    <div class="products">
      <div class="header__of__products">
        <span>Лидеры продаж</span>
        <button class="all_products">все товары</button>
      </div>
      <swiper
        :modules="modules"
        :slides-per-view="2.1"
        :space-between="8"
        :scrollbar="{ draggable: true }"
        @swiper="onSwiper"
        @slideChange="onSlideChange"
      >
        <swiper-slide
          ><div class="product__card">
            <div class="product__header">
              <div>-46%</div>
              <img src="./image/image 1.png" alt="product" />
            </div>
            <div class="product__body">
              <span>Ambassador</span>
              <div>Кофе в зернах Ambassador Nero</div>
            </div>
            <div class="product__footer">
              <span>725 c</span>
              <button>
                <img src="./image/Add to cart.svg" alt="basket" />
              </button>
            </div></div
        ></swiper-slide>
        <swiper-slide
          ><div class="product__card">
            <div class="product__header">
              <div>-46%</div>
              <img src="./image/image 1.png" alt="product" />
            </div>
            <div class="product__body">
              <span>Ambassador</span>
              <div>Кофе в зернах Ambassador Nero</div>
            </div>
            <div class="product__footer">
              <span>725 c</span>
              <button>
                <img src="./image/Add to cart.svg" alt="basket" />
              </button>
            </div></div
        ></swiper-slide>
        <swiper-slide
          ><div class="product__card">
            <div class="product__header">
              <div>-46%</div>
              <img src="./image/image 1.png" alt="product" />
            </div>
            <div class="product__body">
              <span>Ambassador</span>
              <div>Кофе в зернах Ambassador Nero</div>
            </div>
            <div class="product__footer">
              <span>725 c</span>
              <button>
                <img src="./image/Add to cart.svg" alt="basket" />
              </button>
            </div></div
        ></swiper-slide>
        <swiper-slide
          ><div class="product__card">
            <div class="product__header">
              <div>-46%</div>
              <img src="./image/image 1.png" alt="product" />
            </div>
            <div class="product__body">
              <span>Ambassador</span>
              <div>Кофе в зернах Ambassador Nero</div>
            </div>
            <div class="product__footer">
              <span>725 c</span>
              <button>
                <img src="./image/Add to cart.svg" alt="basket" />
              </button>
            </div></div
        ></swiper-slide>
        <swiper-slide
          ><div class="product__card">
            <div class="product__header">
              <div>-46%</div>
              <img src="./image/image 1.png" alt="product" />
            </div>
            <div class="product__body">
              <span>Ambassador</span>
              <div>Кофе в зернах Ambassador Nero</div>
            </div>
            <div class="product__footer">
              <span>725 c</span>
              <button>
                <img src="./image/Add to cart.svg" alt="basket" />
              </button>
            </div></div
        ></swiper-slide>
        <swiper-slide
          ><div class="product__card">
            <div class="product__header">
              <div>-46%</div>
              <img src="./image/image 1.png" alt="product" />
            </div>
            <div class="product__body">
              <span>Ambassador</span>
              <div>Кофе в зернах Ambassador Nero</div>
            </div>
            <div class="product__footer">
              <span>725 c</span>
              <button>
                <img src="./image/Add to cart.svg" alt="basket" />
              </button>
            </div></div
        ></swiper-slide>
      </swiper>
    </div>
  </div>
</template>

<script>
import MyInput from "@/components/MyInput.vue";
import { Swiper, SwiperSlide } from "swiper/vue";
import { Pagination, Autoplay,Scrollbar } from "swiper";

import "swiper/css";
import "swiper/css/pagination";
import "swiper/css/autoplay";
import 'swiper/css/scrollbar';

export default {
  components: { MyInput, Swiper, SwiperSlide },
  setup() {
    return {
      modules: [Pagination, Autoplay,Scrollbar],
    };
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
@font-face {
  font-family: "SF UI Display";
  src: url("./fonts/AnyConv.com__sf-ui-display-semibold.woff2"),
    url("./fonts/AnyConv.com__sf-ui-display-semibold.woff");
  font-weight: 500;
  font-display: swap;
  font-style: normal;
}
@font-face {
  font-family: "SF UI Display";
  src: url("./fonts/AnyConv.com__sf-ui-display-regular.woff2"),
    url("./fonts/AnyConv.com__sf-ui-display-regular.woff");
  font-weight: 400;
  font-display: swap;
  font-style: normal;
}
@font-face {
  font-family: "SF UI Display";
  src: url("./fonts/AnyConv.com__sf-ui-display-bold.woff2"),
    url("./fonts/AnyConv.com__sf-ui-display-bold.woff");
  font-weight: 700;
  font-display: swap;
  font-style: normal;
}
h2 {
  font-family: "SF UI Display";
  font-style: normal;
  font-weight: 500;
  font-size: 22px;
  line-height: 28px;
  margin-bottom: 12px;
}
.search__area {
  background: #f2f2f7;
  padding: 16px;
}
.search__input {
  display: flex;
  align-items: center;
  padding: 8px;
  gap: 10px;
  background: #e3e3e9;
  border-radius: 4px;
}
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
.slider {
  padding: 24px 16px 16px;
}
.slider__baner {
  height: 200px;
  width: 100%;
  border-radius: 4px;
}
.swiper {
  --swiper-theme-color: #fff;
  --swiper-pagination-bullet-inactive-color: rgba(255, 255, 255, 1);
}
.banner__scroll {
  margin: 0 auto;
}
.banners {
  padding: 16px;
}
.banners__content {
  display: grid;
  grid-template: 1fr 1fr/1fr 1fr;
  grid-template-areas:
    "card card"
    "left-side right-side";
  grid-gap: 8px;
}
.banners__content img:nth-child(1) {
  grid-area: card;
}
.banners__content img:nth-child(2) {
  grid-area: left-side;
}
.banners__content img:nth-child(3) {
  grid-area: right-side;
}
.banner_item {
  width: 100%;
  border-radius: 4px;
}
.products {
  padding: 24px 16px;
}
.header__of__products {
  display: flex;
  justify-content: space-between;
}
.header__of__products span {
  font-family: "SF UI Display";
  font-style: normal;
  font-weight: 500;
  font-size: 20px;
  line-height: 26px;
}
.all_products {
  background: transparent;
  border: none;
  color: #2dbe64;
  font-family: "SF UI Display";
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 26px;
}
.product__card {
  display: flex;
  flex-direction: column;
  row-gap: 8px;
  margin: 24px 0 0 0;
}
.product__header {
  display: flex;
  position: relative;
  justify-content: center;
  align-items: center;
  padding: 20px 0;
}
.product__header div:nth-child(1) {
  position: absolute;
  top: 12px;
  right: auto;
  padding: 4px;
  bottom: auto;
  left: 12px;
  color: #ff0000;
  background: #ffd4d4;
  border-radius: 8px;
  font-family: "SF UI Display";
  font-style: normal;
  font-weight: 400;
  font-size: 11px;
  line-height: 12px;
}
.product__header img {
  height: 120px;
}
.product__footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-family: "SF UI Display";
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
  margin-bottom: 24px;
}
.product__footer button {
  border: none;
  background: transparent;
  cursor: pointer;
}
.product__body {
  display: flex;
  flex-direction: column;
  gap: 4px;
}
.product__body div {
  font-family: "SF UI Display";
  font-size: 14px;
  font-weight: 400;
  line-height: 20px;
}
.product__body span {
  font-size: 12px;
  font-weight: 500;
  line-height: 16px;
  color: rgba(60, 60, 67, 0.6);
}
.swiper-horizontal > .swiper-scrollbar,
.swiper-scrollbar.swiper-scrollbar-horizontal{
  height: 2px;
}
</style>
