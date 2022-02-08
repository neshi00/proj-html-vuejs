<template>
  <div id="app">
    <jumbotron-top />
    <!--header interno  -->
    <more-about-section />
    <audiobook-section />

    <footer-box />
  </div>
</template>

<script>
import JumbotronTop from "./components/JumbotronTop.vue";
import FooterBox from "./components/FooterBox.vue";
import MoreAboutSection from "./components/MoreAboutSection.vue";
import AudiobookSection from "./components/AudiobookSection.vue";

export default {
  name: "App",
  components: {
    JumbotronTop,
    FooterBox,
    MoreAboutSection,
    AudiobookSection,
  },
};
</script>

<style lang="scss">
@import "./style/UtilityClass.scss";
</style>
