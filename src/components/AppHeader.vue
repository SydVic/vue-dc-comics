<template>
  <header class="header">
    <div class="header__nav-container">
      <div class="header__nav-container__nav-logo">
        <img src="../assets/img/dc-logo.png" alt="" />
      </div>
      <div class="header__nav-container__nav-menu">
        <ul>
          <li
            v-for="(item, index) in headerLinks"
            :key="index"
            :class="{ active: item.active }"
          >
            <a href="">{{ item.text }}</a>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  data: function () {
    return {
      headerLinks: [
        {
          text: "characters",
          active: false,
        },
        {
          text: "comics",
          active: true,
        },
        {
          text: "movies",
          active: false,
        },
        {
          text: "tv",
          active: false,
        },
        {
          text: "games",
          active: false,
        },
        {
          text: "collectibles",
          active: false,
        },
        {
          text: "videos",
          active: false,
        },
        {
          text: "fans",
          active: false,
        },
        {
          text: "news",
          active: false,
        },
        {
          text: "shop",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/common.scss";
@import "../style/mixin.scss";

.header {
  height: $header-height;
  background-color: $white;
  display: flex;

  align-items: center;

  &__nav-container {
    @include general-container-properties();
    display: flex;
    justify-content: space-between;
    align-items: center;

    &__nav-logo {
      height: 80px;
      width: 80px;

      img {
        width: 100%;
      }
    }

    &__nav-menu {
      ul {
        display: flex;

        li {
          color: $black;
          margin-left: 1rem;
          line-height: calc($header-height - $active-border-bottom);
          border-bottom: $active-border-bottom solid transparent;

          &.active {
            color: $primary-color;
            border-bottom: $active-border-bottom solid $primary-color;
          }

          a {
            color: inherit;
            text-transform: uppercase;
            font-size: 0.7rem;
            font-weight: bold;
          }
        }
      }
    }
  }
}
</style>
