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
    height: 50px;
  }
}
</style>