<template>
  <div class="macro-container">
    <div class="container">
      <div class="logo-box">
        <img src="../assets/author-logo-round.png" alt="logo" />
      </div>

      <div class="links-area">
        <ul>
          <li v-for="data in footerData" :key="data.id">
            <h3>{{ data.category }}</h3>
            <p>
              {{ data.latinus }}
            </p>
            <ul v-for="(link, i) in data.links" :key="i">
              <li>
                <i class="fas fa-angle-right"></i>
                <a href="#">{{ link }}</a>
              </li>
            </ul>

            <ul v-for="(info, i) in data.info" :key="i">
              <li>
                <a href="#">{{ info }}</a>
              </li>
            </ul>
          </li>
        </ul>
      </div>
    </div>
    <dir id="copyright">
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur
        voluptatem
      </p>
    </dir>
  </div>
</template>

<script>
export default {
  components: {},
  props: {
    footerData: Array,
  },
};
</script>

<style lang="scss" scoped>
.macro-container {
  background: url(../assets/hero-07-2x.jpg);
  background-size: cover;
  height: 400px;

  .container {
    display: flex;
    justify-content: space-between;

    .logo-box {
      height: 150px;
      width: 20%;

      img {
        height: 100%;
      }
    }

    .links-area {
      width: 80%;

      ul {
        display: flex;

        i {
          vertical-align: middle;
        }
      }
    }
  }

  #copyright {
    p {
      text-align: center;
    }
  }
}
</style>
