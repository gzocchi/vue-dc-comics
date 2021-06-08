<template>
  <main>
    <Jumbotron />
    <div class="container">
      <div class="gallery">
        <h1>--&#62; Gallery goes here &#60;--</h1>
      </div>
    </div>
  </main>
</template>

<script>
import Jumbotron from "./Jumbotron.vue";
import comics from "../data/dc-comics.js";

export default {
  name: "Main",
  components: {
    Jumbotron,
  },
  data: function () {
    return {
      comics: comics,
    };
  },
};
</script>

<style scoped lang="scss">
@import "../style/variables";

main {
  background-color: $dc_black;

  .gallery {
    height: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
}
</style>