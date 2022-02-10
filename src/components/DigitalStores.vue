<template>
  <div class="macro-container">
    <div class="digital-stores skinny-container">
      <div class="stores-images">
        <img src="../assets/ebay-logotan-2x.png" alt="ebay logo" />
        <img src="../assets/audible-logotan-2x.png" alt="audible logo" />
        <img src="../assets/bb-logotan-2x.png" alt="barnes&noble logo" />
        <img src="../assets/kindlefire-logotan-2x.png" alt="kindle fire logo" />
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
  background-color: $beige-plt;
  padding: 50px 0;

  .stores-images {
    display: flex;
    width: calc(100% / 4);

    img {
      width: 100%;
      padding: 0px 30px;
      cursor: pointer;
    }
  }
}
</style>
