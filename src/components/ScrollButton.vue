<template>
  <div class="macro-container">
    <button @click="$emit('moveUp')">prova</button>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.macro-container {
  position: relative;

  button {
    z-index: 100;
    position: fixed;
    bottom: 0;
    right: 100px;
  }
}
</style>
