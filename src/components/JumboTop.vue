<template>
  <div class="jumbo macro-container">
    <header-box :navLinks="navLinks" />

    <div class="jumbo-container">
      <div class="jumbo-text-box">
        <h1>Damon Vaughn</h1>
        <!--testo strano  -->
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
            <button><i class="fab fa-amazon"></i>Buy On Amazon</button>
            <button><i class="fab fa-apple"></i>Buy On AppStore</button>
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
.jumbo {
  height: 100vh;
  background: url(../assets/hero-07-2x.jpg);
  background-size: cover;
  background-repeat: no-repeat;

  header {
    height: 30%;
  }

  .jumbo-container {
    height: 70%;
    display: flex;

    .jumbo-text-box {
      padding: 150px;
      width: 60%;
      color: #ffffff;

      h1 {
        padding: 10px 0;
      }
      .text {
        width: 70%;
        padding: 10px 0;
      }
      p {
        padding: 10px 0;
      }
      .buttons-box {
        padding: 10px 0;

        button {
          margin: 0 1px;
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
            }
            p {
              padding: 10px 0;
            }
          }
        }

        .buttons-box {
          display: flex;
          padding-top: 20px;

          button {
            width: 50%;
            padding: 5px 20px;

            i {
              padding: 0 10px;
            }
          }
        }
      }
    }
  }
}
</style>
