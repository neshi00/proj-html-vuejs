<template>
  <div class="container">
    <div class="title-section">
      <h3>Upcoming Events</h3>
      <h5>Met the author in person</h5>
    </div>

    <div class="boxes-area">
      <div class="box-one">
        <img src="" alt="" />
        <h4>test</h4>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Commodi ex
          libero dolore, laboriosam ipsa, at labore similique blanditiis hic ut
          ullam itaque numquam quas, iusto quidem illo error ducimus dolorem!
        </p>
      </div>
      <div class="box-two">
        <img src="" alt="" />
        <h4>test</h4>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Commodi ex
          libero dolore, laboriosam ipsa, at labore similique blanditiis hic ut
          ullam itaque numquam quas, iusto quidem illo error ducimus dolorem!
        </p>
      </div>
      <div class="box-three">
        <img src="" alt="" />
        <h4>test</h4>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Commodi ex
          libero dolore, laboriosam ipsa, at labore similique blanditiis hic ut
          ullam itaque numquam quas, iusto quidem illo error ducimus dolorem!
        </p>
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

  .box-one,
  .box-two,
  .box-three {
    width: calc(100% / 3);
  }
}
</style>
