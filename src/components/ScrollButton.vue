<template>
  <div class="macro-container">
    <button>
      <a href="#"><i class="fas fa-angle-up"></i></a>
    </button>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../style/ColorsPalette.scss";

.macro-container {
  position: relative;

  button {
    z-index: 100;
    position: fixed;
    bottom: 0;
    right: 100px;

    background-color: $black-plt;
    opacity: 0.8;
    padding: 10px;
    border-radius: 5px;
  }
}
</style>
