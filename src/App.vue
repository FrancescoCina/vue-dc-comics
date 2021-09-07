<template>
  <div id="app">
    <Header></Header>
    <Products></Products>
    <Navbar></Navbar>
    <Footer></Footer>
    <BottomFooter></BottomFooter>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Products from "@/components/Products.vue";
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
import BottomFooter from "@/components/BottomFooter.vue";

export default {
  name: "App",
  components: {
    Header,
    Products,
    Navbar,
    Footer,
    BottomFooter,
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/style.scss";
</style>
