<template>
  <div>
    <img :src="thumb" alt="series" />
  </div>
</template>

<script>
export default {
  name: "Card",
  props: ["thumb"],
};
</script>

<style lang="scss" scoped>
div {
  max-height: 200px;
  overflow: hidden;

  img {
    width: 100%;
  }
}
</style>
