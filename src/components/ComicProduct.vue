<template>
  <div class="comic-product-card">
    <div class="product-img">
      <img :src="productObj.thumb" alt="productObj.series" />
    </div>
    <div class="product-title">{{ productObj.series }}</div>
  </div>
</template>

<script>
export default {
  name: "ComicsProduct",
  props: {
    productObj: Object,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.comic-product-card {
  width: 200px;
  margin: 3rem 0 2rem 0;

  .product-img {
    width: 200px;
    height: 200px;
    overflow: hidden;
  }

  .product-title {
    color: $white;
    text-transform: uppercase;
    margin-top: 1.5rem;
  }
}
</style>
