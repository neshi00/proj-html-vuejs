<template>
  <div id="app">
    <jumbotron-top />
    <!--header interno  -->
    <more-about-section />
    <audiobook-section />
    <press-section />
    <upcoming-events-section />
    <newsletter-section />
    <deepening-section />
    <recent-articles-section />

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
import NewsletterSection from "./components/NewsletterSection.vue";
import RecentArticlesSection from "./components/RecentArticlesSection.vue";

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
    NewsletterSection,
    RecentArticlesSection,
  },
};
</script>

<style lang="scss">
@import "./style/UtilityClass.scss";
</style>
