<template>
  <div class="macro-container">
    <div class="skinny-container">
      <div class="digital-stores">
        <img src="../assets/ebay-logotan-2x.png" alt="ebay logo" />
        <img src="../assets/audible-logotan-2x.png" alt="audible logo" />
        <img src="../assets/bb-logotan-2x.png" alt="barnes & noble logo" />
        <img src="../assets/kindlefire-logotan-2x.png" alt="kindle fire logo" />
      </div>
      <div class="jumbotron-app">
        <div class="box-image">
          <img src="../assets/audible-app-2x.png" alt="audible app" />
        </div>
        <div class="box-text">
          <h3>New Audiobook</h3>
          <h5>BLABLABLA BLA BLA</h5>
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Amet ad
            eius veritatis perspiciatis officia maxime, obcaecati dolor
            exercitationem recusandae ab dolorem doloremque delectus
            consequuntur omnis pariatur nisi vel. Similique, iste.
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
  .skinny-container {
    border: 5px solid teal;

    .digital-stores {
      width: calc(100% / 4);
      display: flex;

      img {
        width: 100%;
      }
    }

    .jumbotron-app {
      display: flex;

      .box-image {
        width: 50%;
        border: 1px solid green;

        img {
          width: 100%;
        }
      }

      .box-text {
        width: 50%;

        .app-images {
          width: 100%;
          display: flex;

          img {
            width: calc(100% / 3);
          }
        }
      }
    }
  }
}
</style>
