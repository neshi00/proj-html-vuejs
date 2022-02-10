<template>
  <header class="container">
    <div class="logo-box">
      <img src="../assets/author-logo-round.png" alt="logo" />
    </div>

    <nav>
      <ul>
        <li v-for="link in navLinks" :key="link.id">
          <div class="link-nav">
            <a :href="link.url">{{ link.category }}</a>
          </div>
        </li>

        <li>
          <div class="link-nav">
            <a href="#"><i class="fas fa-shopping-cart"></i></a>
          </div>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  props: {
    navLinks: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/ColorsPalette.scss";

header {
  display: flex;
  justify-content: space-between;

  color: #fff;

  .logo-box {
    height: 200px;

    img {
      height: 100%;
    }
  }

  nav {
    // line-height: 100px;

    ul {
      display: flex;

      li {
        padding: 0 20px;

        .link-nav {
          padding: 20px 0;
          border-top: 5px solid transparent;

          &:hover {
            border-top: 5px solid $yellow-plt;
          }
        }
      }
    }
  }
}
</style>
