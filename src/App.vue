<template>
  <div id="app">
    <fixed-buttons />
    <scroll-button />
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
    <footer-box :usefulLinks="usefulLinks" :infoData="infoData" />
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
      // -------------------------data footer
      usefulLinks: [
        "Latest Books",
        "Upcoming Events",
        "Recent Articles",
        "Business Enquiries",
        "Visit My Foundation",
      ],
      infoData: [
        "63 E. Studebaker Street Bolingbrook, IL 60440",
        "Phone: (800)000-0000",
        "Mobile: (800)000-0000",
        "Email:info@your-company.com",
      ],
      // ---------------------------/data footer
    };
  },
};
</script>

<style lang="scss">
@import url("https://use.fontawesome.com/releases/v5.7.1/css/all.css");
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Comforter&display=swap");
@import "./style/UtilityClass.scss";
@import "./style/ColorsPalette.scss";
</style>
