<template>
  <nav>
    <section class="images-container">
      <figure v-for="imglink in imagesLinks" :key="imglink.url">
        <a href="#">
          <img :src="imglink.url" :alt="imglink.name" />
          <figcaption>{{ imglink.name }}</figcaption>
        </a>
      </figure>
    </section>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      imagesLinks: [
        {
          name: "DIGITAL COMICS",
          url: require("@/assets/img/buy-comics-digital-comics.png"),
          current: false,
        },
        {
          name: "DC MERCHANDISE",
          url: require("@/assets/img/buy-comics-merchandise.png"),
          current: true,
        },
        {
          name: "SUBSCRIPTION",
          url: require("@/assets/img/buy-comics-subscriptions.png"),
          current: false,
        },
        {
          name: "COMIC SHOP LOCATOR",
          url: require("@/assets/img/buy-comics-shop-locator.png"),
          current: false,
        },
        {
          name: "DC POWER VISA",
          url: require("@/assets/img/buy-dc-power-visa.svg"),
          current: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "@/assets/scss/_vars.scss";

nav {
  height: 195px;
  background-color: $hero-color;
  position: relative;
  top: 0;
}

.images-container {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  figure {
    width: 70px;
    height: 100px;
    display: flex;
    align-items: center;

    margin-top: 40px;
    a {
      text-decoration: none;
      display: flex;
      align-items: center;
    }
    figcaption {
      color: #fff;
      padding-left: 10px;
    }

    img {
      max-width: 100%;
      height: auto;
    }
  }
}
</style>