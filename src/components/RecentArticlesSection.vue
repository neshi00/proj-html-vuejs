<template>
  <div class="macro-container">
    <div class="container">
      <header>
        <div class="header-text">
          <div>Recent Articles</div>
          <h5>Read the last bla bla bla</h5>
        </div>
        <div class="header-button">
          <button>bla blabla bla</button>
        </div>
      </header>

      <section>
        <div class="macro-box-sx">
          <img src="../assets/20-Tips-scaled.jpg" alt="" />
          <!--todo  -->
          <h2>Best author of blabla</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti
            ipsum expedita ex facere id illum nemo voluptatum sit inventore
            provident enim, ad quod natus ratione laudantium sequi modi pariatur
            tenetur?
          </p>

          <span>Justin Blabla, The Ney York Times</span>
        </div>
        <div class="boxes-dx">
          <div class="box-one">
            <img src="../assets/thumb-13-2x-700x441.jpg" alt="catalog photo" />
            <h4>A true masterpiece, Bravo!</h4>
            <p>
              Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aperiam,
              sequi! Natus veritatis optio ipsam tempora, autem fugiat sapiente
              cumque ullam dolore earum unde quis nisi. Sed eligendi alias quo
              amet?
            </p>
          </div>

          <div class="box-two">
            <img src="../assets/thumb-08-2x-320x202.jpg" alt="book photo" />
            <h4>A Unique view on the world</h4>
            <p>
              Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aperiam,
              sequi! Natus veritatis optio ipsam tempora, autem fugiat sapiente
              cumque ullam dolore earum unde quis nisi. Sed eligendi alias quo
              amet?
            </p>
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
.macro-container {
  background-color: beige;
  header {
    display: flex;
    justify-content: space-between;

    .header-text {
    }

    .header-button {
      line-height: 70px;
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

      p {
        border-top: 1px solid #ffffff;
      }
    }

    .boxes-dx {
      background-color: #ffffff;
      margin-left: 10px;
      width: 40%;
      padding: 20px;

      .box-one,
      .box-two {
        img {
          width: 100%;
        }
        border: 1px solid red;
      }
    }
  }
}
</style>
