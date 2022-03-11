<template>
  <div class="loader wf-section" style="display: none">
    <div class="loader-wrapper">
      <div class="progress-bar-wrapper">
        <div
          class="progress-bar"
          style="
            transform: translate3d(-100%, 0px, 0px) scale3d(1, 1, 1)
              rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
            transform-style: preserve-3d;
          "
        ></div>
      </div>
    </div>
  </div>
  <div class="full-page">
    <Navbar @toggleDropdown="toggleDropdown" :navTitles="navTitles"></Navbar>
    <MainTitleSection :mainTitle="mainTitle">
      <template #test>
        <Promotions :mainTitle="mainTitle"></Promotions>
      </template>
    </MainTitleSection>
    <AboutSection></AboutSection>
    <MarketingSection></MarketingSection>
    <CompanyInfoSection></CompanyInfoSection>
    <CompanyMembers></CompanyMembers>
    <ParticipateSection></ParticipateSection>
    <IndividualAgenda></IndividualAgenda>
    <Footer></Footer>
  </div>
</template>

<script setup>
import Navbar from "./components/NavbarSection/Navbar.vue";
import MainTitleSection from "./components/MainTitleSection.vue";
import AboutSection from "./components/AboutSection/AboutSection.vue";
import MarketingSection from "./components/MarketingSection/MarketingSection.vue";
import CompanyInfoSection from "./components/CompanyInfoSection/CompanyInfoSection.vue";
import CompanyMembers from "./components/CompanyInfoSection/CompanyInfoComponents/CompanyMembers.vue";
import CompanyAgenda from "./components/CompanyInfoSection/CompanyInfoComponents/CompanyAgenda.vue";
import IndividualAgenda from "./components/CompanyInfoSection/CompanyInfoComponents/IndividualAgenda.vue";
import ParticipateSection from "./components/ParticipateSection/ParticipateSection.vue";
import Footer from "./components/FooterSection/Footer.vue";
import Promotions from "./components/MainTitleComponents/Promotions.vue";
import { ref } from "@vue/reactivity";

function test(navTitle) {
  console.log("Test successful!!", navTitle.showDropdown);
}

function toggleDropdown(navTitle) {
  navTitle.showDropdown = !navTitle.showDropdown;
  console.log(navTitle.showDropdown);
}

const navTitles = ref([
  {
    navName: "Landings",
    showDropdown: false,
    subTitleOpen: false,
    navSubTitles: [
      {
        navSubName: "Landing 01",
        navSubPageLink: "https://friday-template.webflow.io/",
      },
      {
        navSubName: "Landing 02",
        navSubPageLink: "https://friday-template.webflow.io/",
      },
      {
        navSubName: "Landing 03",
        navSubPageLink: "https://friday-template.webflow.io/",
      },
      {
        navSubName: "Landing 04",
        navSubPageLink: "https://friday-template.webflow.io/",
      },
      {
        navSubName: "Landing 05",
        navSubPageLink: "https://friday-template.webflow.io/",
      },
    ],
  },
  {
    navName: "Features",
    showDropdown: false,
    subTitleOpen: false,
    navSubTitles: [
      {
        navSubName: "Features 01",
        navSubPageLink: "https://friday-template.webflow.io/",
      },
      {
        navSubName: "Features 02",
        navSubPageLink: "https://friday-template.webflow.io/",
      },
      {
        navSubName: "Features 03",
        navSubPageLink: "https://friday-template.webflow.io/",
      },
      {
        navSubName: "Features 04",
        navSubPageLink: "https://friday-template.webflow.io/",
      },
    ],
  },
  {
    navName: "CMS",
    showDropdown: false,
    subTitleOpen: false,
    navSubTitles: [
      {
        navSubName: "CMS 01",
        navSubPageLink: "https://friday-template.webflow.io/",
      },
      {
        navSubName: "CMS 02",
        navSubPageLink: "https://friday-template.webflow.io/",
      },
      {
        navSubName: "CMS 03",
        navSubPageLink: "https://friday-template.webflow.io/",
      },
    ],
  },
  {
    navName: "Template",
    showDropdown: false,
    subTitleOpen: false,
    navSubTitles: [
      {
        navSubName: "Template 01",
        navSubPageLink: "https://friday-template.webflow.io/",
      },
      {
        navSubName: "Template 02",
        navSubPageLink: "https://friday-template.webflow.io/",
      },
      {
        navSubName: "Template 03",
        navSubPageLink: "https://friday-template.webflow.io/",
      },
      {
        navSubName: "Template 04",
        navSubPageLink: "https://friday-template.webflow.io/",
      },
    ],
  },
]);

// MainTitleSection data
const mainTitle = ref({
  companyFirstName: "Apple",
  eventActivity: "Marathon",
  emojiURL:
    "https://upload.wikimedia.org/wikipedia/commons/thumb/e/e6/Noto_Emoji_KitKat_263a.svg/1200px-Noto_Emoji_KitKat_263a.svg.png",
  joinButtonText: "Join Here",
  learnMoreText: "Click here to learn more",
  promotionText: "Promotion",
});
</script>

<style></style>
