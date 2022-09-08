<template>
  <div>
    <div class="q-pa-md q-gutter-sm">
    <q-toggle
        v-model="first"
        keep-color
        checked-icon="dark_mode"
        color="green"
        unchecked-icon="light_mode"
        @click="themChange"
        size="40px"
      />
    </div>
    <search-area :darkMode="darkMode"/>
    <stories-bar :darkMode="darkMode"/>
    <main-bill-board />
    <banners />
    <products-scroller />
    <brands />
    <store />
    <shorts />
  </div>
</template>

<script>
import SearchArea from "./components/SearchArea.vue";
import StoriesBar from "./components/StoriesBar.vue";
import MainBillBoard from "./components/MainBillBoard.vue";
import Banners from "./components/Banners.vue";
import ProductsScroller from "./components/ProductsScroller.vue";
import Brands from "./components/Brands.vue";
import Store from "./components/Store.vue";
import Shorts from "./components/Shorts.vue";
import { useQuasar } from "quasar";
import { ref } from 'vue';
export default {
  components: {
    SearchArea,
    StoriesBar,
    MainBillBoard,
    Banners,
    ProductsScroller,
    Brands,
    Store,
    Shorts,
  },
  setup() {
    const $q = useQuasar();
    $q.dark.set(false);
    return{
      first: ref(false)
    }
  },
  methods:{
    themChange(){
      this.$q.dark.toggle();
      this.darkMode = this.first;
    }
  },

};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
:root{
  --green:#2DBE64;
  --secondary-light:#F2F2F7;
  --radius:4px;
  --black:#000000;
  --bg-input: rgba(120, 120, 128, 0.32);
  --color-of-text:rgba(235, 235, 245, 0.6);
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
  color:var(--green);
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
