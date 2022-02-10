<template>
  <div class="macro-container">
    <div class="container">
      <div class="title-section">
        <h3>Upcoming Events</h3>
        <h5>MET THE AUTHOR IN PERSON</h5>
      </div>

      <div class="boxes-area">
        <div class="box-one">
          <img src="../assets/event-05.jpg" alt="chicago photo" />
          <h4>Chicago Book Signing</h4>
          <p>
            Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Mauris
            blandit aliquet elit, eget tincidunt nibh pulvinar a nulla.
          </p>
        </div>
        <div class="box-two">
          <img src="../assets/event-04.jpg" alt="testimonial photo" />
          <h4>Meet & Greet With Amanda</h4>
          <p>
            Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a.
            Praesent sapien massa, convallis a pellentesque nec, egestas.
          </p>
        </div>
        <div class="box-three">
          <img src="../assets/event-07.jpg" alt="book photo" />
          <h4>Open Book: Dialogues</h4>
          <p>
            Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Mauris
            blandit aliquet elit, eget tincidunt nibh pulvinar a nulla.
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
  padding: 50px 0;

  .title-section {
    text-align: center;

    h3 {
      padding-bottom: 10px;
    }
    h5 {
      padding-bottom: 30px;
    }
  }

  .boxes-area {
    display: flex;

    .box-one,
    .box-two,
    .box-three {
      width: calc(100% / 3);
      text-align: center;
      background-color: #ffffff;
      margin: 0 20px;

      img {
        width: 100%;

        &:hover {
          filter: contrast(0.6) brightness(125%) saturate(175%);
          transition: all 0.5s;
        }
      }

      h4 {
        padding: 10px 0;
      }

      p {
        border-top: 1px solid gray;
        margin: 10px;
        padding: 10px 0;
      }
    }
  }
}
</style>
