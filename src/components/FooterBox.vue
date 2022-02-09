<template>
  <div class="macro-container">
    <div class="container">
      <div class="logo-box">
        <img src="../assets/author-logo-round.png" alt="logo" />
      </div>

      <div class="links-area">
        <ul class="boxes-footer">
          <li class="single-box" v-for="data in footerData" :key="data.id">
            <h3>{{ data.category }}</h3>
            <p v-if="data.latinus !== null">
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
        Copyright 2012-2020 | Avada Theme by <a href="#">ThemeFusion</a>|All
        Rights Reserved|Powered by <a href="#">WordPress</a>
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
  padding: 50px 0;

  .container {
    display: flex;
    justify-content: space-between;

    .logo-box {
      height: 150px;
      width: 20%;
      padding: 20px;

      img {
        height: 100%;
      }
    }

    .links-area {
      width: 80%;

      .boxes-footer {
        display: flex;

        .single-box {
          width: calc(100% / 3);
          padding: 20px;

          h3 {
            padding: 20px 0;
          }

          i {
            vertical-align: middle;
            padding-right: 15px;
          }

          li {
            padding-bottom: 10px;
          }
        }
      }
    }
  }

  #copyright {
    p {
      text-align: center;
      padding: 10px 0;
    }
  }
}
</style>
