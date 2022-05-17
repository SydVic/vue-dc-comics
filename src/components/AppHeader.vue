<template>
  <header class="header">
    <div class="header__nav-container">prova</div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/mixin.scss";

.header {
  height: $header-height;
  background-color: $white;

  &__nav-container {
    @include general-container-properties();
    background-color: aqua;
  }
}
</style>
