<template>
  <div id="app">
    <Home />
  </div>
</template>

<script>
import Home from "./components/Home.vue";
export default {
  name: "app",
  components: {
    Home
  }
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Heebo:wght@400;700&display=swap");
@import url("https://fonts.googleapis.com/css?family=Noto+Sans+JP:400,700&display=swap");

#app {
  font-family: "Archivo Narrow", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
