<template>
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
              <img src="../image/image 1.png" alt="product" />
            </div>
            <div class="product__body">
              <span>Ambassador</span>
              <div>Кофе в зернах Ambassador Nero</div>
            </div>
            <div class="product__footer">
              <span>725 c</span>
              <button>
                <img src="../image/Add to cart.svg" alt="basket" />
              </button>
            </div></div
        ></swiper-slide>
        <swiper-slide
          ><div class="product__card">
            <div class="product__header">
              <div>-46%</div>
              <img src="../image/image 1.png" alt="product" />
            </div>
            <div class="product__body">
              <span>Ambassador</span>
              <div>Кофе в зернах Ambassador Nero</div>
            </div>
            <div class="product__footer">
              <span>725 c</span>
              <button>
                <img src="../image/Add to cart.svg" alt="basket" />
              </button>
            </div></div
        ></swiper-slide>
        <swiper-slide
          ><div class="product__card">
            <div class="product__header">
              <div>-46%</div>
              <img src="../image/image 1.png" alt="product" />
            </div>
            <div class="product__body">
              <span>Ambassador</span>
              <div>Кофе в зернах Ambassador Nero</div>
            </div>
            <div class="product__footer">
              <span>725 c</span>
              <button>
                <img src="../image/Add to cart.svg" alt="basket" />
              </button>
            </div></div
        ></swiper-slide>
        <swiper-slide
          ><div class="product__card">
            <div class="product__header">
              <div>-46%</div>
              <img src="../image/image 1.png" alt="product" />
            </div>
            <div class="product__body">
              <span>Ambassador</span>
              <div>Кофе в зернах Ambassador Nero</div>
            </div>
            <div class="product__footer">
              <span>725 c</span>
              <button>
                <img src="../image/Add to cart.svg" alt="basket" />
              </button>
            </div></div
        ></swiper-slide>
        <swiper-slide
          ><div class="product__card">
            <div class="product__header">
              <div>-46%</div>
              <img src="../image/image 1.png" alt="product" />
            </div>
            <div class="product__body">
              <span>Ambassador</span>
              <div>Кофе в зернах Ambassador Nero</div>
            </div>
            <div class="product__footer">
              <span>725 c</span>
              <button>
                <img src="../image/Add to cart.svg" alt="basket" />
              </button>
            </div></div
        ></swiper-slide>
        <swiper-slide
          ><div class="product__card">
            <div class="product__header">
              <div>-46%</div>
              <img src="../image/image 1.png" alt="product" />
            </div>
            <div class="product__body">
              <span>Ambassador</span>
              <div>Кофе в зернах Ambassador Nero</div>
            </div>
            <div class="product__footer">
              <span>725 c</span>
              <button>
                <img src="../image/Add to cart.svg" alt="basket" />
              </button>
            </div></div
        ></swiper-slide>
      </swiper>
    </div>
</template>

<script>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Pagination, Autoplay, Scrollbar } from "swiper";
import "swiper/css";
import "swiper/css/pagination";
import "swiper/css/autoplay";
import "swiper/css/scrollbar";
export default {
  components: { Swiper, SwiperSlide },
  setup() {
    return {
      modules: [Pagination, Autoplay, Scrollbar],
    };
  },
};
</script>

<style scoped>
.products {
  padding: 24px 16px;
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
  background: #fff;
  border-radius: 4px;
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

</style>