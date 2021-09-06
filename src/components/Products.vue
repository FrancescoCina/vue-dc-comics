<template>
  <section class="products">
    <div class="container row">
      <div class="col">
        <h2>Content Goes Here</h2>
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
.products {
  margin-top: 20px;
  background-color: #000;
  height: 200px;
  h2 {
    color: #fff;
    font-size: 25px;
  }
}
.col {
  height: 100%;
  display: flex;
  align-items: center;
}
</style>