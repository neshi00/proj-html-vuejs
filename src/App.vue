<template>
  <div id="app">
    <fixed-buttons />
    <scroll-button @click="moveUp" />
    <jumbo-top :navLinks="navLinks" />
    <!--header interno  -->
    <more-about-section />
    <digital-stores />
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
import JumboTop from "./components/JumboTop.vue";
import FooterBox from "./components/FooterBox.vue";
import MoreAboutSection from "./components/MoreAboutSection.vue";
import DigitalStores from "./components/DigitalStores.vue";
import AudiobookSection from "./components/AudiobookSection.vue";
import PressSection from "./components/PressSection.vue";
import UpcomingEventsSection from "./components/UpcomingEventsSection.vue";
import DeepeningSection from "./components/DeepeningSection.vue";
import NewsletterSection from "./components/NewsletterSection.vue";
import RecentArticlesSection from "./components/RecentArticlesSection.vue";
import FixedButtons from "./components/FixedButtons.vue";
import ScrollButton from "./components/ScrollButton.vue";

export default {
  name: "App",
  components: {
    JumboTop,
    FooterBox,
    MoreAboutSection,
    DigitalStores,
    AudiobookSection,
    PressSection,
    UpcomingEventsSection,
    DeepeningSection,
    NewsletterSection,
    RecentArticlesSection,
    FixedButtons,
    ScrollButton,
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
          url: "#",
        },
        {
          id: "4",
          category: "My Blog",
          url: "#",
        },
        {
          id: "5",
          category: "Meetups",
          url: "#",
        },
        {
          id: "6",
          category: "Shop",
          url: "#",
        },
        {
          id: "7",
          category: "Contact Me",
          url: "#",
        },
      ],

      footerData: [
        {
          id: "1",
          category: "ABOUT ME",
          latinus:
            "Vivamus suscipit tortor eget felis porttitor voluptat. Nulla quis lorem ut libero malesuada feugiat. Vivamus suscipit tortor eget felis porttitor voluptat.",
        },
        {
          id: "2",
          category: "USEFUL LINKS",
          latinus: null,
          links: [
            "Latest Books",
            "Upcoming Events",
            "Recent Articles",
            "Business Enquiries",
            "Visit My Foundation",
          ],
        },
        {
          id: "3",
          category: "CONTACT INFO",
          latinus: null,
          info: [
            "63 E. Studebaker Street Bolingbrook, IL 60440",
            "Phone: (800)000-0000",
            "Mobile: (800)000-0000",
            "Email:info@your-company.com",
          ],
        },
      ],
    };
  },
  methods: {
    moveUp() {
      window.scrollTo(0, 0);
    },
  },
};
</script>

<style lang="scss">
@import url("https://use.fontawesome.com/releases/v5.7.1/css/all.css");
@import "./style/UtilityClass.scss";
</style>
