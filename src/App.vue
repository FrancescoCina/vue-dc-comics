<template>
  <div id="app">
    <Header></Header>
    <Products></Products>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Products from "@/components/Products.vue";

export default {
  name: "App",
  components: {
    Header,
    Products,
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/_generics.scss";
@import "@/assets/scss/_utilities.scss";
</style>
