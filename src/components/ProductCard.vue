<template>
  <div class="comics-container">
    <div v-for="(comic, index) in comics" :key="index" class="comic-card">
      <img :src="comic.thumb" :alt="comic.series" />
      <figcaption>{{ comic.series }}</figcaption>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProductCard",
  props: ["comics"],
};
</script>

<style scoped lang="scss">
.comics-container {
  display: flex;
  flex-wrap: wrap;
  .comic-card {
    flex-basis: calc(100% / 6);
    height: calc(100% / 6);
    padding: 25px;
    figcaption {
      color: #fff;
      text-transform: uppercase;
      font-size: 15px;
    }
    img {
      max-width: 100%;
      height: 100%;
    }
  }
}
</style>