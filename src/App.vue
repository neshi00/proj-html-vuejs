<template>
  <div id="app">
    <jumbotron-top />
    <!--header interno  -->

    <footer-box />
  </div>
</template>

<script>
import JumbotronTop from "./components/JumbotronTop.vue";
import FooterBox from "./components/FooterBox.vue";

export default {
  name: "App",
  components: {
    JumbotronTop,
    FooterBox,
  },
};
</script>

<style lang="scss">
@import "./style/UtilityClass.scss";
</style>
