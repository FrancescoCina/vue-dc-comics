<template>
  <header>
    <div class="container">
      <div class="row">
        <div class="logo">
          <img src="@/assets/img/dc-logo.png" alt="Logo" />
        </div>
        <nav>
          <ul class="col">
            <li v-for="link in links" :key="link.text">
              <a :href="link.url">{{ link.text }}</a>
            </li>
          </ul>
        </nav>
      </div>
    </div>
  </header>
</template> 

<script>
export default {
  name: "Header",
  data() {
    return {
      links: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
header {
  height: 120px;
}

.logo {
  margin: 15px;
  width: 200px;
  height: 100%;
}

.logo img {
  max-width: 100%;
  height: auto;
}

ul li {
  list-style-type: none;
  text-transform: uppercase;
  a {
    margin: 0 20px;
    text-decoration: none;
    color: #000;
    font-weight: 600;
    font-size: 1.2rem;
  }
}

a:hover {
  color: #0282f9;
}

.col {
  display: flex;
  justify-content: center;
}
</style>