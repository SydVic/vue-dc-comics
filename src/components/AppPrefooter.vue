<template>
  <section class="pre-footer">
    <div class="pre-footer__container">
      <ul class="icons-list">
        <li>
          <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
          <h3>Digital Comics</h3>
        </li>
        <li>
          <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
          <h3>Digital Comics</h3>
        </li>
        <li>
          <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
          <h3>Digital Comics</h3>
        </li>
        <li>
          <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
          <h3>Digital Comics</h3>
        </li>
        <li>
          <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
          <h3>Digital Comics</h3>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: "AppPrefooter",
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/mixin.scss";
@import "../style/common.scss";

.pre-footer {
  background-color: $primary-color;

  &__container {
    @include general-container-properties();

    .icons-list {
      display: flex;

      li {
        width: calc(100% / 5);
      }
    }
  }
}
</style>
