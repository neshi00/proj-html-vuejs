<template>
  <div class="macro-container">
    <div class="container">
      <header>
        <div class="header-text">
          <h3>Recent Articles</h3>
          <h5>READ THE LATEST ENTRIES</h5>
        </div>
        <div class="header-button">
          <button class="btn-custom">All Articles</button>
        </div>
      </header>

      <section>
        <div class="macro-box-sx">
          <img src="../assets/20-Tips-scaled.jpg" alt="book photo" />
          <div>
            <h4>20 Creativity Tips</h4>

            <p>
              By <b>admin</b> | October 24th, 2019 | Categories: Event, Tips &
              Tricks
            </p>
            <p>
              Vestibulum ante ipsum primis in faucibus orci luctus et ultrices
              posuere cubilia Curae; Donec velit neque, auctor sit amet aliquam
              vel, ullamcorper sit amet.
            </p>
          </div>
        </div>
        <div class="boxes-dx">
          <div class="box-one">
            <img src="../assets/thumb-13-2x-700x441.jpg" alt="catalog photo" />
            <h4>What's On Your Booklist?</h4>
            <p>October 24th, 2019 | 0 Comments</p>
          </div>

          <div class="box-two">
            <img src="../assets/thumb-08-2x-320x202.jpg" alt="book photo" />
            <h4>Instanbul Travel Guide</h4>
            <p>October 24th, 2019 | 0 Comments</p>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../style/ColorsPalette.scss";

.macro-container {
  background-color: $beige-plt;

  header {
    display: flex;
    justify-content: space-between;
    padding: 30px 20px;

    .header-text {
      h5 {
        color: $green-plt;
        padding: 10px 0;
      }
    }

    .header-button {
      margin: auto 0;

      button {
        background-color: $yellow-plt;
        border: 1px solid $yellow-plt;
        color: #ffffff;

        &:hover {
          background-color: $brown-plt;
          border: 1px solid $brown-plt;
          transition: all 0.5s;
        }
      }
    }
  }

  section {
    display: flex;
    padding: 20px;

    .macro-box-sx {
      background-color: #ffffff;
      margin-right: 10px;
      height: 750px;
      width: 70%;
      padding: 20px;

      img {
        width: 100%;
      }

      div {
        padding-right: 50px;

        h4 {
          padding-top: 10px;
        }

        p {
          padding: 10px 0;
          color: $gray-plt;
        }
      }
    }

    .boxes-dx {
      background-color: #ffffff;
      margin-left: 10px;
      width: 30%;
      padding: 20px;

      .box-one,
      .box-two {
        height: 50%;

        img {
          width: 100%;
        }

        h4 {
          padding: 10px 0;
        }

        p {
          padding-bottom: 10px;
          color: $gray-plt;
        }
      }
    }
  }
}
</style>
