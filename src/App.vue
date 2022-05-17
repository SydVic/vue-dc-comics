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
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

body {
  background-color: #000000;
}
</style>
