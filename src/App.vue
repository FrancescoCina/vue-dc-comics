<template>
  <div id="app">
    <Header></Header>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
export default {
  name: "App",
  components: {
    Header,
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/_generics.scss";
@import "@/assets/scss/_utilities.scss";
</style>
