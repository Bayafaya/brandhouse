<template>
  <div class="search__area">
    <div class="search__input">
      <img src="../image/ri-search-2-line.svg" alt="search" />
      <my-input type="text" placeholder="Поиск товара" />
    </div>
  </div>
</template>

<script>
import MyInput from './UI/MyInput.vue';
export default {
  components: { MyInput },

};
</script>

<style scoped>
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
</style>
