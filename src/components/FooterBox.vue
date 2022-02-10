<template>
  <div class="macro-container">
    <div class="container">
      <div class="logo-box">
        <img src="../assets/author-logo-round.png" alt="logo" />
      </div>

      <div class="links-area">
        <div class="boxes-footer">
          <div class="single-box">
            <h3>ABOUT ME</h3>
            <p>
              Vivamus suscipit tortor eget felis porttitor voluptat. Nulla quis
              lorem ut libero malesuada feugiat. Vivamus suscipit tortor eget
              felis porttitor voluptat.
            </p>
          </div>

          <div class="single-box">
            <h3>USEFUL LINKS</h3>
            <ul v-for="(link, i) in usefulLinks" :key="i">
              <li>
                <a href="#"><i class="fas fa-angle-right"></i>{{ link }}</a>
              </li>
            </ul>
          </div>

          <div class="single-box">
            <h3>CONTACT INFO</h3>
            <ul v-for="(info, i) in infoData" :key="i">
              <li>{{ info }}</li>
            </ul>
            <div class="social-icons">
              <i class="fab fa-facebook"> </i>
              <i class="fab fa-twitter"></i>
              <i class="fab fa-instagram"></i>
              <i class="fab fa-linkedin"></i>
              <i class="fab fa-youtube"></i>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="box-bottom container">
      <p>
        Copyright 2012-2020 | Avada Theme by
        <a href="#"><span>ThemeFusion</span></a
        >|All Rights Reserved|Powered by <a href="#"><span>WordPress</span></a>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  props: {
    usefulLinks: Array,
    infoData: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/ColorsPalette.scss";

.macro-container {
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url(../assets/hero-07-2x.jpg);
  background-size: cover;
  padding: 50px 0;

  .container {
    display: flex;
    justify-content: space-between;

    .logo-box {
      height: 200px;
      width: 20%;

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
          padding: 0 20px;

          h3 {
            padding: 20px 0;
            color: #ffffff;
          }

          li {
            color: $lightgray-plt;
          }

          p {
            color: $lightgray-plt;
          }

          i {
            vertical-align: middle;
            padding-right: 15px;
            cursor: pointer;
          }

          .social-icons {
            padding: 20px 0;
            color: $lightgray-plt;

            i {
              color: $lightgray-plt;

              &:hover {
                color: #ffffff;
              }
            }
          }
        }
      }
    }
  }
  .box-bottom {
    color: $lightgray-plt;
    padding: 50px 0;

    p {
      margin: 0 auto;

      span {
        color: #ffffff;
      }
    }
  }
}
</style>
