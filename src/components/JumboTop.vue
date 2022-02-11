<template>
  <div class="jumbo macro-container">
    <header-box :navLinks="navLinks" />

    <div class="jumbo-container">
      <div class="jumbo-text-box">
        <h1>Damon Vaughn</h1>

        <div class="text">
          Best-selling author and the most influential public intellectual in
          the western world right now.
        </div>
        <p>- The New York Times</p>
        <div class="buttons-box">
          <button><i class="fas fa-arrow-left"></i></button>
          <button><i class="fas fa-arrow-right"></i></button>
        </div>
      </div>

      <div class="latest-release">
        <div class="inner-box">
          <div class="box-flex">
            <div class="widget-microbox">
              <img src="../assets/book-widget.png" alt="" />
            </div>
            <div class="widget-text">
              <h3>Latest Book Release</h3>
              <h5>D. VAUGHN AUTOBIOGRAPHY</h5>
              <p>
                Vestibulum tristique turpis in ipsum egestas lobortis. Duis
                maximus bibendum voluptat. Lorem ipsum dolor sit amet.
              </p>
            </div>
          </div>
          <div class="buttons-box">
            <button class="btn-custom">
              <i class="fab fa-amazon"></i>Buy On Amazon
            </button>
            <button class="btn-custom">
              <i class="fab fa-apple"></i>Buy On AppStore
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import HeaderBox from "./HeaderBox.vue";

export default {
  components: {
    HeaderBox,
  },
  props: {
    navLinks: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/ColorsPalette.scss";

.jumbo {
  height: 100vh;
  background-image: linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.4)),
    url(../assets/hero-07-2x.jpg);
  background-size: cover;

  header {
    height: 20%;
  }

  .jumbo-container {
    height: 80%;
    display: flex;

    .jumbo-text-box {
      padding: 100px 0 200px 200px;
      width: 60%;
      color: #ffffff;

      h1 {
        padding: 10px 0;
      }
      .text {
        width: 70%;
        padding: 10px 0;
        font-size: 40px;
      }
      p {
        padding: 10px 0;
        color: $lightgray-plt;
      }
      .buttons-box {
        padding: 10px 0;

        button {
          margin: 0 1px;
          background-color: $black-plt;
          opacity: 0.8;
          padding: 8px;
          border-radius: 5px;
        }
      }
    }

    .latest-release {
      position: relative;
      width: 40%;

      .inner-box {
        background-color: #ffffff;
        position: absolute;
        bottom: 0;
        padding: 30px;

        .box-flex {
          display: flex;

          .widget-microbox {
            width: 50%;

            img {
              width: 100%;
            }
          }

          .widget-text {
            width: 50%;

            h3 {
              padding: 10px 0;
            }
            h5 {
              padding: 10px 0;
              color: $yellow-plt;
            }
            p {
              padding: 10px 0;
              color: $gray-plt;
            }
          }
        }

        .buttons-box {
          display: flex;
          padding-top: 20px;

          button {
            width: 50%;
            border: 1px solid $green-plt;
            border-radius: 5px;

            &:hover {
              background-color: $green-plt;
              color: #ffffff;
              transition: all 0.5s;
              i {
                color: #ffffff;
                transition: all 0.5s;
              }
            }

            i {
              padding: 0 10px;
              color: $black-plt;
            }
          }
        }
      }
    }
  }
}
</style>
