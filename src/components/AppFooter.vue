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
    <section class="footer__bottom">
      <div class="footer__bottom__container">
        <div class="cta-btn-wrapper">
          <a href="">sign-up now!</a>
        </div>
        <div class="social-contacts-wrapper">
          <div class="follow-us">follow us</div>
          <ul class="social-list">
            <li>
              <a href="">
                <img src="../assets/img/footer-facebook.png" alt="" />
              </a>
            </li>
            <li>
              <a href="">
                <img src="../assets/img/footer-twitter.png" alt="" />
              </a>
            </li>
            <li>
              <a href="">
                <img src="../assets/img/footer-youtube.png" alt="" />
              </a>
            </li>
            <li>
              <a href="">
                <img src="../assets/img/footer-pinterest.png" alt="" />
              </a>
            </li>
            <li>
              <a href="">
                <img src="../assets/img/footer-periscope.png" alt="" />
              </a>
            </li>
          </ul>
        </div>
      </div>
    </section>
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

  &__bottom {
    height: 100px;
    background-color: $dark-grey;
    display: flex;
    align-items: center;

    &__container {
      @include general-container-properties();
      display: flex;
      justify-content: space-between;
      align-items: center;

      .cta-btn-wrapper {
        display: inline-block;
        border: 2px solid $primary-color;

        a {
          display: inline-block;
          color: $white;
          font-weight: 600;
          text-transform: uppercase;
          padding: 0.7rem 0.7rem;
        }
      }
    }
  }

  .social-contacts-wrapper {
    display: flex;
    align-items: center;

    .follow-us {
      color: $primary-color;
      text-transform: uppercase;
      font-weight: 600;
    }

    .social-list {
      li {
        display: inline-block;
        margin-left: 0.8rem;

        a {
          font-size: 0.8rem;
        }
      }
    }
  }
}
</style>
