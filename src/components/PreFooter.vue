<template>
  <section class="pre-footer">
    <div class="pre-footer__container">icons</div>
  </section>
</template>

<script>
export default {
  name: "PreFooter",
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/mixin.scss";

.pre-footer {
  height: $pre-footer-height;
  background-color: $primary-color;

  &__container {
    @include general-container-properties();
    /*test*/
    border: 1px solid white;
    height: 100%;
  }
}
</style>
