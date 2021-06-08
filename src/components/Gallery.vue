<template>
  <div id="gallery">
    <div v-for="(comic, index) in comics" :key="index" class="gallery_card">
      <a :href="comic.thumb" target="_blank">
        <Card :thumb="comic.thumb" />
        <p>{{ comic.series }}</p>
      </a>
    </div>
    <a href="#gallery" class="btn">Load More </a>
  </div>
</template>

<script>
import Card from "./Card.vue";
import comics from "../data/dc-comics.js";

export default {
  name: "Gallery",
  components: {
    Card,
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

#gallery {
  display: flex;
  flex-wrap: wrap;
  padding: 40px 0 20px;
  text-transform: uppercase;

  a {
    text-decoration: none;
    color: inherit;
  }
  .gallery_card {
    flex-shrink: 0;
    width: calc(100% / 6);
    padding: 10px;

    p {
      margin: 10px 0;
      font-size: 0.9em;
    }
  }
}

.btn {
  padding: 10px 50px;
  margin: 10px auto 0;
  background-color: $dc_blue;
  font-weight: 700;
}
</style>