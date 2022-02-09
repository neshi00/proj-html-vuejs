<template>
  <div id="app">
    <jumbotron-top :navLinks="navLinks" />
    <!--header interno  -->
    <more-about-section />
    <audiobook-section />
    <press-section />
    <upcoming-events-section />
    <newsletter-section />
    <deepening-section />
    <recent-articles-section />

    <footer-box :footerData="footerData" />
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
  data() {
    return {
      navLinks: [
        {
          id: "1",
          category: "Home",
          url: "#",
        },
        {
          id: "2",
          category: "About Me",
          url: "#",
        },
        {
          id: "3",
          category: "Testimonials",
        },
        {
          id: "4",
          category: "My Blog",
        },
        {
          id: "5",
          category: "Meetups",
        },
        {
          id: "6",
          category: "Shop",
        },
        {
          id: "7",
          category: "Contact Me",
        },
      ],

      footerData: [
        {
          id: "1",
          category: "ABOUT ME",
          latinus:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa",
        },
        {
          id: "2",
          category: "USEFUL LINKS",
          latinus:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa",
          links: ["info1", "info2", "info3"],
        },
        {
          id: "3",
          category: "CONTACT INFO",
          latinus:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa",
          info: ["info1", "info2", "info3"],
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import url("https://use.fontawesome.com/releases/v5.7.1/css/all.css");
@import "./style/UtilityClass.scss";
</style>
