<template>
  <section class="bottom-footer">
    <div class="row">
      <div class="col">
        <div class="sign-up">
          <h5><a href="#">SIGN UP NOW!</a></h5>
        </div>
      </div>
      <div class="col"></div>
    </div>
  </section>
</template>

<script>
export default {
  name: "BottomFooter",
};
</script>

<style>
.bottom-footer {
  background-color: #303030;
}

.col {
  flex-basis: 50%;
}

.sign-up {
  border: 1px solid #0282f9;
}
</style>