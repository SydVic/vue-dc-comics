<template>
  <div id="app">
    <AppHeader />
    <main>
      <AppJumbotron />
      <ComicsSlide />
    </main>
    <AppPrefooter />
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppJumbotron from "./components/AppJumbotron.vue";
import ComicsSlide from "./components/ComicsSlide.vue";
import AppPrefooter from "./components/AppPrefooter.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppJumbotron,
    ComicsSlide,
    AppPrefooter,
    AppFooter,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
@import "./style/variables.scss";

main {
  background-color: #000000;
}
/*test*/
</style>
