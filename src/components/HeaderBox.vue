<template>
  <header class="container">
    <div class="logo-box">
      <img src="../assets/author-logo-round.png" alt="logo" />
    </div>

    <nav>
      <ul>
        <li><a href="#">testo</a></li>
        <li>testo</li>
        <li>testo</li>
        <li>testo</li>
        <li>testo</li>
        <li>testo</li>
        <li>testo</li>
        <li>carrello</li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {};
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
