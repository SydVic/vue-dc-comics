<template>
  <section class="pre-footer">
    <div class="pre-footer__container">icons</div>
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

.pre-footer {
  /*test*/
  height: $pre-footer-height;
  /*test*/
  background-color: $primary-color;

  &__container {
    @include general-container-properties();
  }
}
</style>
