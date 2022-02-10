<template>
  <div class="container">
    <header>
      <div class="header-text">
        <h3>What The Critics Say</h3>
        <h5>TESTIMONIALS FROM AROUND THE WORLD</h5>
      </div>
      <div class="header-button">
        <button class="btn-custom">Read All Testimonials</button>
      </div>
    </header>

    <section>
      <div class="macro-box-sx">
        <h2>Best Author Of His Generation</h2>
        <p>This book will change your perspective on life</p>
        <p>
          Donec fringilla nunc eu turpis dignissim, at euismod sapien tincidunt.
          Maecenas eleifend congue cursus. In vitae enim quis sem pharetra.
          Curabitur ercu erat, accumsan id imperdiet et, porttitor at sem
        </p>
        <p>
          Donec rutrum congue leo eget malesuada. Vivamus suscipit tortor eget
          felis porttitor voluptat. Nulla quis lorem ut liber. Proin eget tortor
          risus. Praesent sapien massa, convallis a pellentesque nec, egestas
          non nisi. Donec rutrum congue leo eget malesuada.
        </p>
        <img
          src="../assets/nytimes-logo-white-xsmall.png"
          alt="the new york times logo"
        />
        <span>Justin Kilpatrick, The Ney York Times</span>
      </div>
      <div class="boxes-dx">
        <div class="box-one">
          <h4>A True Masterpiece, Bravo!</h4>
          <p>
            Nulla quis lorem ut libero malesuada feugiat. Vivamus magna justo,
            lacinia eget consectetur sed, convallis at tellus. Vivamus suscipit
            tortor eget felis porttitor voluptat. Nulla quis lorem ut libero
            malesuada feug at.
          </p>
        </div>
        <div class="signature">
          <img src="../assets/theguardian-xsmall.png" alt="the guardian logo" />
          <span>Gerald Hendley, The Guardian</span>
        </div>

        <div class="box-two">
          <h4>A Unique View On The World</h4>
          <p>
            Donec sollicitudin molestie malesuada. Curabitur arcu erat, accumsan
            id imperdiet et, porttitor at sem. Vestibulum ac diam sit amet quam
            vehicula elementum sed sit amet dui. Nulla quis lorem ut libero
            malesuada feugiat. Vestibulum ac diam amet.
          </p>
        </div>
        <div class="signature">
          <img src="../assets/globe-xsmall.png" alt="globe logo" />
          <span>Mary Blabla, The Globe and Mail</span>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container {
  padding: 50px;

  header {
    display: flex;
    justify-content: space-between;
    margin: 30px 0;

    .header-text {
      h3 {
        padding: 10px 0;
      }
      h5 {
        padding: 10px 0;
        color: green;
      }
    }

    .header-button {
      margin: auto 0;
      padding: 0 100px;

      button {
        background-color: orange;
        color: #ffffff;
      }
    }
  }

  section {
    display: flex;

    .macro-box-sx {
      background-image: linear-gradient(rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.2)),
        url(../assets/testimonial2-2x.jpg);
      background-position-y: -100px;
      background-size: cover;
      color: #ffffff;
      width: 60%;
      padding: 100px;
      border-bottom-right-radius: 100px;

      h2 {
        padding: 10px 0;
      }

      p {
        padding: 10px 0;
      }

      img {
        vertical-align: middle;
        padding-right: 10px;
      }
    }

    .boxes-dx {
      width: 40%;
      padding: 0 100px;

      img {
        vertical-align: middle;
        padding-right: 10px;
      }

      .box-one,
      .box-two {
        background-color: beige;
        padding: 20px;

        h4 {
          padding: 10px 0;
        }
        p {
          padding: 10px 0;
        }
      }
      .signature {
        margin-bottom: 30px;
      }
    }
  }
}
</style>
