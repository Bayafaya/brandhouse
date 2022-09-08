<template>
  <div class="search__area">
    <div class="search__input">
      <img src="../image/ri-search-2-line.svg" alt="search" />
      <my-input type="text" placeholder="Поиск товара" :darkMode="darkMode"/>
    </div>
  </div>
</template>

<script>
import MyInput from './UI/MyInput.vue';
export default {
  components: { MyInput },
  props: {
    darkMode: {
      type: Boolean,
      required: true,
    },
  },
  watch: {
    darkMode(newValue) {
      if (newValue) {
        const current = document.getElementsByClassName("search__area");
        current[0].classList.toggle("dark");
        const searchInputDark = document.getElementsByClassName("search__input");
        searchInputDark[0].classList.toggle("dark__input");
        const searchInputText = document.getElementsByClassName("input");
        searchInputText[0].classList.toggle("text__input");
      } else {
        const current = document.getElementsByClassName("search__area");
        current[0].classList.toggle("dark");
        const searchInputDark = document.getElementsByClassName("search__input");
        searchInputDark[0].classList.toggle("dark__input");
        const searchInputText = document.getElementsByClassName("input");
        searchInputText[0].classList.toggle("text__input");
      }
    },
  },

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
.dark {
  background: var(--black);
}
.dark__input{
  background: var(--bg-input);
}
.text__input{
  color: var(--color-of-text);
}
</style>
