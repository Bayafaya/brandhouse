<template>
  <input type="text" class="input" :value="modelValue" @input="updateInput" />
</template>

<script>
export default {
  props: {
    modelValue: [String, Number],
  },
  methods: {
    updateInput(e) {
      this.$emit("update:modelValue", e.target.value);
    },
  },
};
</script>

<style scoped>
.input {
  background: transparent;
  border: none;
  font-family: "SF UI Display";
  font-style: normal;
  color: rgba(60, 60, 67, 0.6);
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
  width: 100%;
}
</style>
