<template>
  <section class="bottom-footer">
    <div class="container">
      <div class="row h-100p">
        <div class="col">
          <div class="sign-up">
            <h5><a href="#">SIGN UP NOW!</a></h5>
          </div>
        </div>
        <div class="col">
          <h4>Follow Us</h4>
          <img src="@/assets/img/footer-facebook.png" alt="Logo Facebook" />
          <img src="@/assets/img/footer-twitter.png" alt="Logo Twitter" />
          <img src="@/assets/img/footer-youtube.png" alt="Logo YouTube" />
          <img src="@/assets/img/footer-pinterest.png" alt="Logo Pinteres" />
          <img src="@/assets/img/footer-periscope.png" alt="Logo Periscope" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "BottomFooter",
};
</script>

<style scoped lang="scss">
.bottom-footer {
  background-color: #303030;
  height: 100px;
  position: relative;
  bottom: 0;
}

.col {
  flex-basis: 50%;
  display: flex;
}

.h-100p {
  height: 100px;
}

.sign-up {
  border: 1px solid #0282f9;
  width: 20%;
}

h5 {
  text-align: center;
  padding: 5px;
  font-size: 20px;
  vertical-align: middle;
}

.sign-up {
  border: 1px solid #0282f9;
  width: 15%;
}

a {
  margin-bottom: 50px 0;
  text-decoration: none;
  color: #fff;
  font-size: 0.5rem;
  font-size: 12px;
}

h4 {
  color: #0282f9;
  text-transform: uppercase;
  font-size: 20px;
}

.col img {
  margin: 0 15px;
}
</style>