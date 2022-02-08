<template>
  <div class="macro-container">
    <div class="container">
      <div class="title-section">
        <h3>Upcoming Events</h3>
        <h5>Met the author in person</h5>
      </div>

      <div class="boxes-area">
        <div class="box-one">
          <img src="../assets/event-05.jpg" alt="chicago photo" />
          <h4>test</h4>
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Commodi ex
            libero dolore, laboriosam ipsa, at labore similique blanditiis hic
            ut ullam itaque numquam quas, iusto quidem illo error ducimus
            dolorem!
          </p>
        </div>
        <div class="box-two">
          <img src="../assets/event-04.jpg" alt="testimonial photo" />
          <h4>test</h4>
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Commodi ex
            libero dolore, laboriosam ipsa, at labore similique blanditiis hic
            ut ullam itaque numquam quas, iusto quidem illo error ducimus
            dolorem!
          </p>
        </div>
        <div class="box-three">
          <img src="../assets/event-07.jpg" alt="book photo" />
          <h4>test</h4>
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Commodi ex
            libero dolore, laboriosam ipsa, at labore similique blanditiis hic
            ut ullam itaque numquam quas, iusto quidem illo error ducimus
            dolorem!
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.macro-container {
  background-color: beige;

  .title-section {
    text-align: center;
  }

  .boxes-area {
    display: flex;

    .box-one,
    .box-two,
    .box-three {
      width: calc(100% / 3);
      text-align: center;
      padding: 0 10px;

      img {
        width: 100%;
      }

      p {
        border-top: 1px solid gray;
      }
    }
  }
}
</style>
