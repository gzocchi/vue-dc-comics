<template>
  <header>
    <div class="container">
      <a href="#">
        <img src="../assets/img/dc-logo.png" alt="DC Logo" />
      </a>
      <ul>
        <li v-for="(link, index) in links" :key="index">
          <a :href="link.url" :class="{ active: link.active }">
            {{ link.text }}
          </a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  data: function () {
    return {
      links: [
        {
          text: "Characters",
          url: "#characters",
          active: false,
        },
        {
          text: "Comics",
          url: "#comics",
          active: true,
        },
        {
          text: "Movies",
          url: "#movies",
          active: false,
        },
        {
          text: "Tv",
          url: "#tv",
          active: false,
        },
        {
          text: "Games",
          url: "#games",
          active: false,
        },
        {
          text: "Collectbles",
          url: "#collectibles",
          active: false,
        },
        {
          text: "Videos",
          url: "#videos",
          active: false,
        },
        {
          text: "Fans",
          url: "#fans",
          active: false,
        },
        {
          text: "News",
          url: "#news",
          active: false,
        },
        {
          text: "Shop",
          url: "#shop",
          active: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../style/variables";

header {
  height: 80px;
  background-color: #fff;

  div {
    display: flex;
    justify-content: space-between;
    align-items: center;

    img {
      height: 60px;
    }

    ul {
      display: flex;
      list-style: none;

      li {
        height: 100%;

        &:not(:first-child) {
          margin-left: 15px;
        }

        a {
          height: 100%;
        //   display: inline-block;
          text-decoration: none;
          text-transform: uppercase;
          border-bottom: 4px solid transparent;
          color: $dc_black;

          &.active {
            border-bottom: 4px solid $dc_blue;
            color: $dc_blue;
          }
          &:hover:not(.active) {
            color: $dc_blue;
          }
        }
      }
    }
  }
}
</style>