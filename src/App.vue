<template>
  <div id="app">
    <Header></Header>
    <Products></Products>
    <Footer></Footer>
    <BottomFooter></BottomFooter>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Products from "@/components/Products.vue";
import Footer from "@/components/Footer.vue";
import BottomFooter from "@/components/BottomFooter.vue";

export default {
  name: "App",
  components: {
    Header,
    Products,
    Footer,
    BottomFooter,
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/_generics.scss";
@import "@/assets/scss/_utilities.scss";
</style>
