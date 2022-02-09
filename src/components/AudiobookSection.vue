<template>
  <div class="macro-container">
    <div class="skinny-container">
      <div class="jumbotron-app">
        <div class="box-image">
          <img src="../assets/audible-app-2x.png" alt="audible app" />
        </div>
        <div class="box-text">
          <h3>New Audiobook</h3>
          <h5>NO TIME TO READ? NO PROBLEM. LISTEN TO IT</h5>
          <p>
            Donec fringilla nunc eu turpis dignissim, at euismod sapien
            tincidunt. Maecenas eleifend congue cursus.
          </p>
          <div class="app-images">
            <img src="../assets/audible-logo.png" alt="audible logo app" />
            <img
              src="../assets/bn-logo-tall.png"
              alt="barnes & noble logo app"
            />
            <img
              src="../assets/kindle-logo-tall.png"
              alt="kindle fire logo app"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.macro-container {
  background: url(../assets/banner.jpg);
  background-size: cover;

  .jumbotron-app {
    display: flex;

    .box-image {
      width: 50%;

      img {
        width: 100%;
      }
    }

    .box-text {
      width: 50%;
      margin: auto 0;
      padding: 50px;
      text-align: center;

      h3 {
        color: #ffffff;
        padding: 10px 0;
      }
      h5 {
        color: orange;
        padding: 10px 0;
      }
      p {
        color: lightgray;
        padding: 10px 0;
      }

      .app-images {
        width: 100%;
        display: flex;

        img {
          width: calc(100% / 3);
          padding: 20px;
        }
      }
    }
  }
}
</style>
