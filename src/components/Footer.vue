<template>
  <footer>
    <section class="footer_link">
      <div class="container">
        <div class="list">
          <div class="list_block">
            <h3>dc comics</h3>
            <ul>
              <li>
                <a href="#">Characters</a>
              </li>
              <li>
                <a href="#">Comics</a>
              </li>
              <li>
                <a href="#">Movies</a>
              </li>
              <li>
                <a href="#">TV</a>
              </li>
              <li>
                <a href="#">Games</a>
              </li>
              <li>
                <a href="#">Video</a>
              </li>
              <li>
                <a href="#">News</a>
              </li>
            </ul>
          </div>

          <div class="list_block">
            <h3>Shop</h3>
            <ul>
              <li>
                <a href="#">Shop DC</a>
              </li>
              <li>
                <a href="#">Shop DC Collectibles</a>
              </li>
            </ul>
          </div>

          <div class="list_block">
            <h3>dc</h3>
            <ul>
              <li>
                <a href="#">Terms Of Use</a>
              </li>
              <li>
                <a href="#">Privacy policy (New)</a>
              </li>
              <li>
                <a href="#">Ad Choices</a>
              </li>
              <li>
                <a href="#">Advertising</a>
              </li>
              <li>
                <a href="#">Jobs</a>
              </li>
              <li>
                <a href="#">Subscriptions</a>
              </li>
              <li>
                <a href="#">Talent Workshops</a>
              </li>
              <li>
                <a href="#">CPSC Certificates</a>
              </li>
              <li>
                <a href="#">Ratings</a>
              </li>
              <li>
                <a href="#">Shop Help</a>
              </li>
              <li>
                <a href="#">Contact Us</a>
              </li>
            </ul>
          </div>

          <div class="list_block">
            <h3>Sites</h3>
            <ul>
              <li>
                <a href="#">DC</a>
              </li>
              <li>
                <a href="#">MAD Magazine</a>
              </li>
              <li>
                <a href="#">DC Kids</a>
              </li>
              <li>
                <a href="#">DC Universe</a>
              </li>
              <li>
                <a href="#">DC Power Visa</a>
              </li>
            </ul>
          </div>
        </div>

        <div class="dc_logo">
          <img src="../assets/img/dc-logo-bg.png" alt="DC Logo" />
        </div>
      </div>
    </section>

    <section class="follow">
      <div class="container">
        <div class="sign_up">
          <a href="#">sign-up now!</a>
        </div>

        <div class="social">
          <a href="#">follow us</a>
          <a href="#">
            <img src="../assets/img/footer-facebook.png" alt="facebook" />
          </a>
          <a href="#">
            <img src="../assets/img/footer-twitter.png" alt="twitter" />
          </a>
          <a href="#">
            <img src="../assets/img/footer-youtube.png" alt="youtube" />
          </a>
          <a href="#">
            <img src="../assets/img/footer-pinterest.png" alt="pinterest" />
          </a>
          <a href="#">
            <img src="../assets/img/footer-periscope.png" alt="periscope" />
          </a>
        </div>
      </div>
    </section>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped lang="scss">
@import "../style/variables";

footer {
  section.footer_link {
    background-image: url(../assets/img/footer-bg.jpg);
    background-position: top;
    background-size: cover;
    height: 300px;

    .container {
      display: flex;
      justify-content: space-between;

      div.list {
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        width: 40%;
        padding: 10px 0;

        .list_block {
          padding: 10px;
          padding-left: 0;
          // color: $text_color;

          h3 {
            margin-bottom: 10px;
            text-transform: uppercase;
          }
          ul {
            list-style: none;
          }
          a {
            text-decoration: none;
            font-weight: 400;
            font-size: 0.9em;
            color: rgba($text_color, 0.5);

            &:hover {
              text-decoration: underline;
            }
          }
        }
      }

      div.dc_logo {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 40%;
        overflow: hidden;

        img {
          width: 100%;
        }
      }
    }
  }
  section.follow {
    padding: 20px;
    background-color: rgba($dc-black, 0.9);
    font-weight: 700;

    .container {
      display: flex;
      justify-content: space-between;

      .sign_up {
        display: flex;
        align-items: center;

        a {
          padding: 5px 10px;
          text-transform: uppercase;
          text-decoration: none;
          color: inherit;
          border: 2px solid $dc_blue;

          &:hover {
            background-color: #fff;
            color: $dc_blue;
          }
        }
      }

      .social {
        display: flex;
        align-items: center;

        a {
          margin-left: 10px;

          &:first-child {
            padding: 5px 10px;
            border: 2px solid transparent;
            text-transform: uppercase;
            text-decoration: none;
            color: $dc_blue;

            &:hover {
              background-color: #fff;
              border: 2px solid $dc_blue;
            }
          }

          img {
            height: 100%;
          }
        }
      }
    }
  }
}
</style>