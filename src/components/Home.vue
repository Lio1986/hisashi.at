<template>
  <div class="home">
    <div class="w-25 p-3 mb-1">
      <h1>hi·sa·shi</h1>
    </div>

    <img
      class="img-fluid main-image"
      src="../assets/hisashiAT_main_image.png"
    />
  </div>
</template>

<script>
export default {
  name: "Home"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  font-weight: 700;
}

.main-image {
  position: absolute;
  top: 40%;
}

@media (min-width: 576px) {
  .main-image {
    top: 30%;
  }
}

@media (min-width: 992px) {
  .main-image {
    top: 20%;
  }
}
</style>
