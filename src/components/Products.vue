<template>
  <section class="products">
    <div class="container h-100">
      <div class="row h-100">
        <div class="col h-100">
          <h2>Content Goes Here</h2>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Products",
};
</script>

<style scoped lang="scss">
@import "@/assets/scss/_mixins.scss";

.products {
  background-color: #000;
  height: 150px;
  h2 {
    color: #fff;
    font-size: 25px;
  }
}
.col {
  height: 100%;
  @include center("vertical");
}
</style>