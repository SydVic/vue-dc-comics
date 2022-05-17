<template>
  <footer class="footer">
    <section class="footer__top">
      <div class="footer__top__col">
        <h3>dc comics</h3>
        <ul>
          <li>Characters</li>
          <li>Comics</li>
          <li>Movies</li>
          <li>TV</li>
          <li>Games</li>
          <li>Videos</li>
          <li>News</li>
        </ul>
        <h3>shop</h3>
        <ul>
          <li>Shp DC</li>
          <li>Shop DC Collectibles</li>
        </ul>
      </div>
      <div class="footer__top__col">
        <h3>DC</h3>
        <ul>
          <li>Terms Of Use</li>
          <li>Privacy Policy (New)</li>
          <li>Ad Choices</li>
          <li>Advertising</li>
          <li>Jobs</li>
          <li>Subscriptions</li>
          <li>Talent Workshoops</li>
          <li>CPSC Certificates</li>
          <li>Ratings</li>
          <li>Shop Help</li>
          <li>Contact Us</li>
        </ul>
      </div>
      <div class="footer__top__col">
        <h3>sites</h3>
        <ul>
          <li>DC</li>
          <li>Mad Magazine</li>
          <li>DC Kids</li>
          <li>DC Universe</li>
          <li>DC Power Visa</li>
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
        }
      }
    }
    &__logo-wrapper {
      margin-left: auto;
    }
  }
}
</style>
