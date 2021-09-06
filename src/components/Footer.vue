<template>
  <footer>
    <div class="container">
      <div class="row">
        <div class="col">
          <nav class="row">
            <div class="left-list">
              <ul>
                <h5>DC COMICS</h5>
                <li v-for="link in links" :key="link.text">
                  <a href="link.url">{{ link.text }}</a>
                </li>
              </ul>
              <ul>
                <h5>SHOP</h5>
                <li><a href="#">Sop DC</a></li>
                <li><a href="#">Shop DC Collections</a></li>
              </ul>
            </div>
            <div class="center-list">
              <ul>
                <h5>DC</h5>
                <li v-for="(link, index) in footerLinksDc" :key="index">
                  <a :href="link.url">{{ link.text }}</a>
                </li>
              </ul>
            </div>
            <div class="right-list">
              <ul>
                <h5>SITES</h5>
                <li v-for="(link, index) in sitesLinks" :key="index">
                  <a :href="link.url">{{ link.text }}</a>
                </li>
              </ul>
            </div>
          </nav>
        </div>
        <div class="col">
          <figure>
            <img src="../assets/img/dc-logo-bg.png" alt="Logo" />
          </figure>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
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
      footerLinksDc: [
        {
          text: "Terms Of Use",
          url: "#",
          current: false,
        },
        {
          text: "Privacy Policy (New)",
          url: "#",
          current: false,
        },
        {
          text: "Ad Choices",
          url: "#",
          current: false,
        },
        {
          text: "Advertising",
          url: "#",
          current: false,
        },
        {
          text: "Jobs",
          url: "#",
          current: false,
        },
        {
          text: "Subscriptions",
          url: "#",
          current: false,
        },
        {
          text: "Talent Workshops",
          url: "#",
          current: false,
        },
        {
          text: "CPSC Certificates",
          url: "#",
          current: false,
        },
        {
          text: "Ratings",
          url: "#",
          current: false,
        },
        {
          text: "Shop Help",
          url: "#",
          current: false,
        },
        {
          text: "Contact Us",
          url: "#",
          current: false,
        },
      ],
      sitesLinks: [
        {
          text: "DC",
          url: "#",
          current: false,
        },
        {
          text: "MAD Magazine",
          url: "#",
          current: false,
        },
        {
          text: "DC Kids",
          url: "#",
          current: false,
        },
        {
          text: "DC Universe",
          url: "#",
          current: false,
        },
        {
          text: "DC Power Visa",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
footer {
  height: 500px;
  width: 100%;
  background-image: url("../assets/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
.col {
  flex-basis: 50%;
  figure {
    margin-left: 100px;
  }
}

ul li {
  list-style-type: none;
  a {
    margin-bottom: 50px 0;
    text-decoration: none;
    color: #7a7a7a;
    font-size: 0.5rem;
    font-size: 12px;
  }
}

h5 {
  text-transform: uppercase;
  font-size: 20px;
  color: #fff;
  padding: 20px 0;
}
</style>