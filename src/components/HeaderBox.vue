<template>
  <header class="container">
    <div class="logo-box">
      <img src="../assets/author-logo-round.png" alt="logo" />
    </div>

    <nav>
      <ul>
        <li v-for="link in navLinks" :key="link.id">
          <a :href="link.url">{{ link.category }}</a>
        </li>

        <li>
          <a href="#"><i class="fas fa-shopping-cart"></i></a>
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
    line-height: 100px;

    ul {
      display: flex;

      li {
        padding: 0 5px;
      }
    }
  }
}
</style>
