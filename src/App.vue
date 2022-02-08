<template>
  <div id="app">
    <jumbotron-top />
    <!--header interno  -->
    <more-about-section />
    <audiobook-section />
    <press-section />
    <upcoming-events-section />

    <deepening-section />

    <footer-box />
  </div>
</template>

<script>
import JumbotronTop from "./components/JumbotronTop.vue";
import FooterBox from "./components/FooterBox.vue";
import MoreAboutSection from "./components/MoreAboutSection.vue";
import AudiobookSection from "./components/AudiobookSection.vue";
import PressSection from "./components/PressSection.vue";
import UpcomingEventsSection from "./components/UpcomingEventsSection.vue";
import DeepeningSection from "./components/DeepeningSection.vue";

export default {
  name: "App",
  components: {
    JumbotronTop,
    FooterBox,
    MoreAboutSection,
    AudiobookSection,
    PressSection,
    UpcomingEventsSection,
    DeepeningSection,
  },
};
</script>

<style lang="scss">
@import "./style/UtilityClass.scss";
</style>
