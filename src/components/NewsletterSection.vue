<template>
  <div class="macro-container">
    <div class="skinny-container">
      <section>
        <h3>Subscribe To My Newsletter</h3>
        <h5>BE NOTIFIED ABOUT BOOK SIGNING TOUR DATES</h5>

        <div class="box-buttons">
          <input type="text" placeholder="Insert your mail ...*" />
          <button class="btn-custom">Subscribe</button>
        </div>
        <p>
          Donec fringilla nunc eu turpis dignissim, at euismod sapien tincidunt.
        </p>
      </section>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.macro-container {
  background: url(../assets/banner-2.jpg);
  background-size: cover;
  padding: 100px 0;

  section {
    width: 40%;
    margin: 0 auto;
    text-align: center;
    padding: 30px;

    h3 {
      color: #ffffff;
      padding: 10px 0;
    }
    h5 {
      color: orange;
      padding: 10px 0;
    }

    .box-buttons {
      display: flex;
      justify-content: center;
      padding: 10px 0;

      input {
        width: 70%;
      }

      button {
        width: 30%;
        background-color: lightgreen;
        margin-left: 10px;
      }
    }
    p {
      color: lightgray;
      padding: 10px 0;
    }
  }
}
</style>
