<template>
  <div class="macro-container">
    <div class="buttons-box">
      <div class="button-one">
        <button>
          <i class="fas fa-folder-open"></i>
          <p>Demos</p>
        </button>
      </div>
      <div class="button-two">
        <button>
          <i class="fas fa-dollar-sign"></i>
          <span>39</span>
          <p>On Sale</p>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../style/ColorsPalette.scss";

.macro-container {
  position: relative;

  .buttons-box {
    position: fixed;
    right: 0;
    z-index: 100;
    margin: 70px 10px 0 0;

    .button-one,
    .button-two {
      button {
        width: 65px;
        border-radius: 5px;
        margin: 3px 0;
        padding: 10px 5px;
        box-shadow: -10px -2px 15px 0px rgba(0, 0, 0, 0.45);

        p {
          font-weight: bold;
          font-size: 10px;
        }

        span {
          color: $green-plt;
        }
      }
    }

    .button-one {
      i {
        color: $black-plt;
      }
    }

    .button-two {
      i {
        font-size: 8px;
        vertical-align: top;
        padding: 1px;
        color: $green-plt;
      }
    }
  }
}
</style>
