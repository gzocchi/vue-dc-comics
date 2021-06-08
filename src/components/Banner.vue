<template>
  <section>
    <div class="container">
      <a href="#">
        <img
          src="../assets/img/buy-comics-digital-comics.png"
          alt="Digital Comics"
        />
        <h3>Digital Comics</h3>
      </a>
      <a href="#">
        <img src="../assets/img/buy-comics-merchandise.png" alt="Merchandise" />
        <h3>DC Merchandise</h3>
      </a>
      <a href="#">
        <img
          src="../assets/img/buy-comics-subscriptions.png"
          alt="Subscriptions"
        />
        <h3>Subscriptions</h3>
      </a>
      <a href="#">
        <img
          src="../assets/img/buy-comics-shop-locator.png"
          alt="Shop Locator"
        />
        <h3>Comic Shop Locator</h3>
      </a>
      <a href="#">
        <img src="../assets/img/buy-dc-power-visa.svg" alt="Power Visa" />
        <h3>DC Power Visa</h3>
      </a>
    </div>
  </section>
</template>

<script>
export default {
  name: "Banner",
};
</script>

<style scoped lang="scss">
@import "../style/variables";

section {
  background-color: $dc_blue;

  .container {
    display: flex;
    // justify-content: center;
    padding: 30px 0;

    a {
      display: flex;
      justify-content: center;
      align-items: center;
      text-decoration: none;
      width: 20%;
      color: inherit;

      &:hover {
        text-decoration: underline;
      }

      img {
        max-width: 20%;
        max-height: 50px;
      }

      h3 {
        margin-left: 10px;
        text-transform: uppercase;
        font-weight: 400;
        font-size: 0.9em;
      }
    }
  }
}
</style>