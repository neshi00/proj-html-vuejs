<template>
  <div class="container">
    <h1>More About Damon Vaughn</h1>
    <!--testo strano  -->
    <p>
      Damon Vaughn is a professor of psychology at the University of Toronto, a
      clinical psychologist and the author of the multi-million copy bestseller
      "The story of my life."
    </p>

    <div>
      <button class="btn-custom">Meet The Author</button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../style/ColorsPalette.scss";

.container {
  text-align: center;
  padding: 50px 0;

  h1 {
    padding: 10px 0;
  }
  p {
    padding: 10px 0;
  }
  div {
    padding: 10px 0 30px 0;

    button {
      background-color: $green-plt;
      color: #ffffff;
      border: 1px solid $green-plt;

      &:hover {
        background-color: $darkGreen-plt;
        border: 1px solid $darkGreen-plt;
        transition: all 0.5s;
      }
    }
  }
}
</style>
