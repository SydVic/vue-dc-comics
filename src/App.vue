<template>
  <div id="app">
    <AppHeader />
    <main>qui andrà il contenuto</main>
    <!-- FOOTER -->
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";

export default {
  name: "App",
  components: {
    AppHeader,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";

/* test*/
body {
  background-color: #000000;
}
</style>
