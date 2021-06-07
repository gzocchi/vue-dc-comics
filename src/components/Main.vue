<template>
  <main>
    <div class="container">
      <h1>--&#62; Content goes here &#60;--</h1>
    </div>
  </main>
</template>

<script>
export default {
  name: "Main",
};
</script>

<style scoped lang="scss">
@import "../style/variables";

main {
  height: 100px;
  background-color: $dc_black;

  div {
    display: flex;
    align-items: center;
  }
}
</style>