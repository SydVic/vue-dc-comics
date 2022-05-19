<template>
  <section class="pre-footer">
    <div class="pre-footer__container">
      <ul class="icons-list">
        <li v-for="(item, index) in icons" :key="index">
          <!-- require serve quando inserisci l'immagine in maniera dinamica per far si che venga appunto "richiesta e passata" al browser -->
          <img :src="require(`../assets/img/${item.img}`)" alt="" />
          <h3>{{ item.text }}</h3>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: "AppPrefooter",
  data: function () {
    return {
      icons: [
        {
          img: "buy-comics-digital-comics.png",
          text: "Digital Comics",
        },
        {
          img: "buy-comics-merchandise.png",
          text: "DC merchandise",
        },
        {
          img: "buy-comics-subscriptions.png",
          text: "Subscritpion",
        },
        {
          img: "buy-comics-shop-locator.png",
          text: "Comic Shop Locator",
        },
        {
          img: "buy-dc-power-visa.svg",
          text: "DC Power Visa",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/mixin.scss";
@import "../style/common.scss";

.pre-footer {
  background-color: $primary-color;
  padding: 2rem 2rem;

  &__container {
    @include general-container-properties();

    .icons-list {
      display: flex;

      li {
        width: calc(100% / 5);
        display: flex;
        align-items: center;

        img {
          width: 20%;
        }

        h3 {
          color: $white;
        }
      }
    }
  }
}
</style>
