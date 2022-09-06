<template>
  <div class="banners">
    <div class="banners__content">
      <img class="banner_item" src="../image/banner1.png" alt="banners" />
      <img class="banner_item" src="../image/banner2.png" alt="banners" />
      <img class="banner_item" src="../image/banner3.png" alt="banners" />
    </div>
  </div>
</template>

<script>
export default {

};
</script>

<style scoped>
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
</style>
