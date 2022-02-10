<template>
  <div class="container">
    <div class="title-section">
      <h3>Dig A Little Deeper Into Damon Vaughn</h3>
      <h5>FIND OUT MORE ABOUT THE AUTHOR HIMSELF</h5>
    </div>

    <div class="boxes-area">
      <div class="box-one">
        <div class="text-box">
          <h4>About Me</h4>
          <hr />
          <p>Vesibulum ante ipsum primis</p>
        </div>
      </div>
      <div class="box-two">
        <div class="text-box">
          <h4>My Latest Book</h4>
          <hr />
          <p>Vesibulum ante ipsum primis</p>
        </div>
      </div>
      <div class="box-three">
        <div class="text-box">
          <h4>Book Signing</h4>
          <hr />
          <p>Vesibulum ante ipsum primis</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../style/ColorsPalette.scss";

.container {
  padding-bottom: 50px;

  .title-section {
    text-align: center;
    padding: 20px 0;

    h3 {
      padding-top: 10px;
    }

    h5 {
      padding: 10px 0;
      color: $green-plt;
    }
  }

  .boxes-area {
    display: flex;
    height: 400px;

    .box-one,
    .box-two,
    .box-three {
      position: relative;
      width: calc(100% / 3);
      margin: 0 20px;
      border-bottom-right-radius: 100px;

      &:hover {
        transform: translateY(-10px);
        transition: all 0.5s;
        box-shadow: -10px -2px 15px 0px rgba(0, 0, 0, 0.45);
      }

      .text-box {
        position: absolute;
        transform: translate(-50%, -50%);
        bottom: 0;
        left: 50%;
        text-align: center;

        h4 {
          color: #ffffff;
          padding: 10px 0;
        }
        hr {
          width: 20%;
          margin: 0 auto;
        }
        .border-custom {
          border-bottom: 1px solid black;
          width: 40px;
          text-align: center;
        }
        p {
          color: $yellow-plt;
          padding: 10px 0;
          border-top-width: 5px;
        }
      }
    }

    .box-one {
      background-image: linear-gradient(rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.2)),
        url(../assets/box-1.jpg);
    }
    .box-two {
      background-image: linear-gradient(rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.2)),
        url(../assets/box-4.jpg);
    }
    .box-three {
      background-image: linear-gradient(rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.2)),
        url(../assets/box-3.jpg);
    }
  }
}
</style>
