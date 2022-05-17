<template>
  <footer class="footer">
    <section class="footer__top">
      <div class="footer__top__col">
        <h3>dc comics</h3>
        <ul>
          <li>
            <a href="">Characters</a>
          </li>
          <li>
            <a href="">Comics</a>
          </li>
          <li>
            <a href="">Movies</a>
          </li>
          <li>
            <a href="">TV</a>
          </li>
          <li>
            <a href="">Games</a>
          </li>
          <li>
            <a href="">Videos</a>
          </li>
          <li>
            <a href="">News</a>
          </li>
        </ul>
        <h3>shop</h3>
        <ul>
          <li>
            <a href="">Shop DC</a>
          </li>
          <li>
            <a href="">Shop DC Collectibles</a>
          </li>
        </ul>
      </div>
      <div class="footer__top__col">
        <h3>DC</h3>
        <ul>
          <li>
            <a href="">Terms Of Use</a>
          </li>
          <li>
            <a href="">Privacy Policy (New)</a>
          </li>
          <li>
            <a href="">Ad Choices</a>
          </li>
          <li>
            <a href="">Advertising</a>
          </li>
          <li>
            <a href="">Jobs</a>
          </li>
          <li>
            <a href="">Subscriptions</a>
          </li>
          <li>
            <a href="">Talent Workshops</a>
          </li>
          <li>
            <a href="">CPSC Certificates</a>
          </li>
          <li>
            <a href="">Ratings</a>
          </li>
          <li>
            <a href="">Shop Help</a>
          </li>
          <li>
            <a href="">Contact Us</a>
          </li>
        </ul>
      </div>
      <div class="footer__top__col">
        <h3>sites</h3>
        <ul>
          <li>
            <a href="">DC</a>
          </li>
          <li>
            <a href="">Mad Magazine</a>
          </li>
          <li>
            <a href="">DC Kids</a>
          </li>
          <li>
            <a href="">DC Universe</a>
          </li>
          <li>
            <a href="">DC Power Visa</a>
          </li>
        </ul>
      </div>
      <div class="footer__top__logo-wrapper">
        <img src="../assets/img/dc-logo-bg.png" alt="" />
      </div>
    </section>
    <section class="footer__bottom"></section>
  </footer>
</template>

<script>
export default {
  name: "AppFooter",
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/mixin.scss";
@import "../style/common.scss";

.footer {
  background-image: url("../assets/img/footer-bg.jpg");
  overflow: hidden;

  &__top {
    @include general-container-properties();
    display: flex;

    &__col {
      margin-right: 2rem;

      h3 {
        color: $white;
        text-transform: uppercase;
        margin: 1.5rem 0;
      }
      ul {
        li {
          color: $grey;
          margin-bottom: 0.5rem;

          a {
            color: inherit;
          }
        }
      }
    }
    &__logo-wrapper {
      margin-left: auto;
    }
  }
}
</style>
