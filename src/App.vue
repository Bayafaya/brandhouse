<template>
  <div>
    <search-area/>
    <stories-bar/>
    <main-bill-board/>
    <banners/>
    <products-scroller/>
    <brands/>
    <store/>
    <shorts/>
  </div>
</template>

<script>
import MyInput from "@/components/UI/MyInput.vue";
import { Swiper, SwiperSlide } from "swiper/vue";
import { Pagination, Autoplay, Scrollbar } from "swiper";

import "swiper/css";
import "swiper/css/pagination";
import "swiper/css/autoplay";
import "swiper/css/scrollbar";
import SearchArea from "./components/SearchArea.vue";
import StoriesBar from "./components/StoriesBar.vue";
import MainBillBoard from "./components/MainBillBoard.vue";
import Banners from "./components/Banners.vue";
import ProductsScroller from "./components/ProductsScroller.vue";
import Brands from "./components/Brands.vue";
import Store from "./components/Store.vue";
import Shorts from "./components/Shorts.vue";

export default {
  components: { MyInput, Swiper, SwiperSlide, SearchArea, StoriesBar, MainBillBoard, Banners, ProductsScroller, Brands, Store, Shorts },
  setup() {
    return {
      modules: [Pagination, Autoplay, Scrollbar],
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

.swiper {
  --swiper-theme-color: #fff;
  --swiper-pagination-bullet-inactive-color: rgba(255, 255, 255, 1);
}
.swiper-scrollbar.swiper-scrollbar-horizontal {
  height: 2px;
}
.header__of__products {
  display: flex;
  justify-content: space-between;
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
.header__of__products span {
  font-family: "SF UI Display";
  font-style: normal;
  font-weight: 500;
  font-size: 20px;
  line-height: 26px;
}
</style>
