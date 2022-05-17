<template>
  <div id="app">
    <AppHeader />
    <main>qui andrà il contenuto</main>
    <PreFooter />
    <!-- FOOTER -->
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import PreFooter from "./components/PreFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    PreFooter,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
@import "./style/variables.scss";

/* test*/
body {
  background-color: #000000;
}
main {
  color: $white;
  height: $main-height;
  display: flex;
  align-items: center;
  justify-content: center;
}
/*test*/
</style>
