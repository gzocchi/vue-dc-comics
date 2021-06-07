<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<style lang="scss">
body {
  font-family: 'Roboto', sans-serif;
  font-size: 14px;
}
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
.container {
  width: 80%;
  height: 100%;
  margin: 0 auto;
}
</style>
