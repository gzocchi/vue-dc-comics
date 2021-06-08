<template>
  <main>
    <Jumbotron />
    <div class="container">
      <h1>current series</h1>
      <Gallery />
    </div>
  </main>
</template>

<script>
import Jumbotron from "./Jumbotron.vue";
import Gallery from "./Gallery.vue";

export default {
  name: "Main",
  components: {
    Jumbotron,
    Gallery,
  },
};
</script>

<style scoped lang="scss">
@import "../style/variables";

main {
  background-color: $dc_black;

  & > .container {
    position: relative;

    h1 {
      position: absolute;
      left: 0;
      transform: translateY(-50%);
      padding: 10px 20px;
      background-color: $dc_blue;
      text-transform: uppercase;
    }
  }
}
</style>