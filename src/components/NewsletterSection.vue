<template>
  <div class="macro-container">
    <div class="skinny-container">
      <section>
        <h3>Subscribe To My Newsletter</h3>
        <h5>Be Notified ABOUT BOOK BLA BLA BLA</h5>

        <div class="box-buttons">
          <input type="text" placeholder="blablabla" />
          <button>due</button>
        </div>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit.
          Necessitatibus velit tenetur totam nemo expedita? Dolore quo tempora
          praesentium, fugit rem, quidem obcaecati aspernatur sit assumenda
          dolorum nam ipsa! Eveniet, unde.
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
  height: 400px;

  section {
    width: 40%;
    margin: 0 auto;
    border: 5px solid turquoise;
    text-align: center;

    .box-buttons {
      display: flex;
      justify-content: center;
    }
  }
}
</style>
