<template>
  <button @click="onClick" :style="{ color: color }">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: String,
    color: String,
  },
  methods: {
    onClick() {
      console.log("click");
    },
  },
};
</script>

<style>
button {
  padding: 8px 10px;
  background: rgb(36, 194, 194);
  border: none;
  border-radius: 15px;
  font-size: 16px;
  font-weight: 550;
}
</style>
