<template>
  <div class="container">
    <header>
      <div class="header-text">
        <div>What The Critics Say</div>
        <h5>Tesimonial from around world</h5>
      </div>
      <div class="header-button">
        <button>bla blabla bla</button>
      </div>
    </header>

    <section>
      <div class="macro-box-sx">
        <h2>Best author of blabla</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti
          ipsum expedita ex facere id illum nemo voluptatum sit inventore
          provident enim, ad quod natus ratione laudantium sequi modi pariatur
          tenetur?
        </p>
        <img
          src="../assets/nytimes-logo-white-xsmall.png"
          alt="the new york times logo"
        />
        <span>Justin Blabla, The Ney York Times</span>
      </div>
      <div class="boxes-dx">
        <div class="box-one">
          <h4>A true masterpiece, Bravo!</h4>
          <p>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aperiam,
            sequi! Natus veritatis optio ipsam tempora, autem fugiat sapiente
            cumque ullam dolore earum unde quis nisi. Sed eligendi alias quo
            amet?
          </p>
        </div>
        <div>
          <img src="../assets/theguardian-xsmall.png" alt="the guardian logo" />
          <span>Gerald Blabla, The Guardian</span>
        </div>
        <div class="box-two">
          <h4>A Unique view on the world</h4>
          <p>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aperiam,
            sequi! Natus veritatis optio ipsam tempora, autem fugiat sapiente
            cumque ullam dolore earum unde quis nisi. Sed eligendi alias quo
            amet?
          </p>
          <div>
            <img src="../assets/globe-xsmall.png" alt="globe logo" />
            <span>Mary Blabla, The Globe and Mail</span>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
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

  .macro-box-sx {
    background: url(../assets/testimonial2-2x.jpg);
    background-size: cover;
    color: #ffffff;
    height: 750px;
    width: 60%;

    p {
      border-top: 1px solid #ffffff;
    }
  }

  .boxes-dx {
    width: 40%;

    .box-one {
      border: 1px solid red;
    }
  }
}
</style>
