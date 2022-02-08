<template>
  <div class="jumbo">
    <header-box />

    <div class="jumbo-container">
      <div class="jumbo-text-box">
        <h2>Damon Blabla</h2>
        <!--testo strano  -->
        <div class="text">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ut, velit
          dolorem? Vero iusto dolore mollitia, quae illum autem fuga natus
          suscipit tenetur ipsa, eum corporis iste, quod qui quaerat sequi?
        </div>
        <p>The New York Times</p>
        <div>
          <button>freccia sx</button>
          <button>freccia dx</button>
        </div>
      </div>

      <div class="latest-release">
        <div class="inner-box">
          <div class="box-flex">
            <div class="widget-microbox">
              test
              <img src="../assets/book-widget.png" alt="" />
            </div>
            <div class="widget-text">
              <h3>testo</h3>
              <p>AUTOBIOGRAPHY</p>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam
                quos inventore porro, in, saepe ipsam, facilis pariatur hic
                nostrum quasi illo neque blanditiis ullam odio accusamus.
                Tempore provident qui recusandae?
              </p>
            </div>
          </div>
          <div class="button-box">
            <button>sx</button>
            <button>dx</button>
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
};
</script>

<style lang="scss" scoped>
.jumbo {
  border: 5px solid blue;
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
      width: 60%;

      border: 5px solid yellow;
      color: #ffffff;
    }

    .latest-release {
      position: relative;
      width: 40%;
      border: 5px solid green;

      .inner-box {
        background-color: #ffffff;
        position: absolute;
        bottom: 0;
        border: 5px solid coral;

        .box-flex {
          display: flex;

          .widget-microbox {
            border: 3px solid cadetblue;
            width: 50%;

            img {
              width: 100%;
            }
          }

          .widget-text {
            width: 50%;
          }
        }

        .button-box {
          display: flex;

          button {
            width: 50%;
          }
        }
      }
    }
  }
}
</style>
