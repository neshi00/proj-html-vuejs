<template>
  <div class="container">
    <div class="title-section">
      <h3>Upcoming Events</h3>
      <h5>Met the author in person</h5>
    </div>

    <div class="boxes-area">
      <div class="box-one">
        <div class="text-box">
          <h4>test</h4>
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Commodi ex
            libero dolore, laboriosam ipsa, at labore similique blanditiis hic
            ut ullam itaque numquam quas, iusto quidem illo error ducimus
            dolorem!
          </p>
        </div>
      </div>
      <div class="box-two">
        <div class="text-box">
          <h4>test</h4>
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Commodi ex
            libero dolore, laboriosam ipsa, at labore similique blanditiis hic
            ut ullam itaque numquam quas, iusto quidem illo error ducimus
            dolorem!
          </p>
        </div>
      </div>
      <div class="box-three">
        <div class="text-box">
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
.title-section {
  text-align: center;
}

.boxes-area {
  display: flex;
  height: 400px;

  .box-one,
  .box-two,
  .box-three {
    position: relative;
    width: calc(100% / 3);

    .text-box {
      position: absolute;
      bottom: 0;
    }
  }

  .box-one {
    background: url(../assets/box-1.jpg);
  }
  .box-two {
    background: url(../assets/box-4.jpg);
  }
  .box-three {
    background: url(../assets/box-3.jpg);
  }
}
</style>
