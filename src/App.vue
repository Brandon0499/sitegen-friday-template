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
    <AboutSection :about="about"></AboutSection>
    <MarketingSection :marketing="marketing"></MarketingSection>
    <CompanyInfoSection :companyInfo="companyInfo"></CompanyInfoSection>
    <ParticipateSection :participate="participate"></ParticipateSection>
    <Footer></Footer>
  </div>
</template>

<script setup>
import Navbar from "./components/NavbarSection/Navbar.vue";
import MainTitleSection from "./components/MainTitleSection.vue";
import AboutSection from "./components/AboutSection.vue";
import MarketingSection from "./components/MarketingSection.vue";
import CompanyInfoSection from "./modules/Company/sections/CompanyInfoSection.vue";
import ParticipateSection from "./components/ParticipateSection.vue";
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

// About data
const about = ref({
  companyFullName: "Friday Festival",
  companySlogan: "Together Towards Tomorrow",
  companySummary:
    "Friday Festival is the community driven conference for design team leads, UX/UI designer, Creatives, and Art Directors looking to improve themselves and their teams.",
  statistics: [
    {
      statisticNumbers: "25+",
      statisticFor: "Innovators speakers",
    },
    {
      statisticNumbers: "32",
      statisticFor: "International sponsors",
    },
    {
      statisticNumbers: "18",
      statisticFor: "Creative Workshops",
    },
  ],
  sponsors: [
    {
      sponsorImageURL:
        "/assets/61e5bb75ba3a7e67f00bd4e6_Combined Shape Copy 31.svg",
    },
    {
      sponsorImageURL:
        "/assets/61e5bb75ba3a7e86360bd4eb_LOGO-001-GRAY Copy.svg",
    },
    {
      sponsorImageURL:
        "/assets/61e5bb75ba3a7e474f0bd4ea_Combined Shape Copy 30.svg",
    },
    {
      sponsorImageURL:
        "/assets/61e5bb75ba3a7e3e010bd4e9_Combined Shape Copy 29.svg",
    },
    {
      sponsorImageURL:
        "/assets/61e5bb75ba3a7ea1400bd4e8_Combined Shape Copy 32.svg",
    },
    {
      sponsorImageURL:
        "/assets/61e5bb75ba3a7ebc9e0bd4e7_Combined Shape Copy 28.svg",
    },
    {
      sponsorImageURL:
        "/assets/61e5bb75ba3a7e76a20bd4e5_Combined Shape Copy 27.svg",
    },
  ],
});

// Marketing data
const marketing = ref({
  whyUsText: "Why Attend Friday festival?",
  reasons: [
    {
      reasonTitle: "Raise your skillset to the next level.",
      reasonParagraph:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique.1",
    },
    {
      reasonTitle: "Extend your industry connections.",
      reasonParagraph:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique.2",
    },
    {
      reasonTitle: "Interact live with world-class experts.",
      reasonParagraph:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique.3",
    },
  ],
});

// CompanyInformation data
const companyInfo = ref({
  memberTextAs: "Members",
  membersIntro: "Stay tuned for more annocemeents in the coming months",
  members: [
    {
      memberName: "James Hetfield",
      memberProfileLink:
        "https://friday-template.webflow.io/speakers/james-hetfield",
      memberImageURL:
        "/assets/61fdc09d23a662eecb14d82a_portrait-happy-smiley-man.jpg",
    },
    {
      memberName: "Ada Lovelace",
      memberProfileLink:
        "https://friday-template.webflow.io/speakers/ada-lovelace",
      memberImageURL:
        "https://assets.website-files.com/61e5bb75ba3a7e1b1d0bd3e5/61fdc0a871a096ee4ef00abd_portrait-good-.jpg",
    },
    {
      memberName: "Tiffany Tattum",
      memberProfileLink:
        "https://friday-template.webflow.io/speakers/tiffany-tattum",
      memberImageURL:
        "https://assets.website-files.com/61e5bb75ba3a7e1b1d0bd3e5/61fdc767a1b84ad984911b54_pretty-smiling-joyfully-female-with-fair-hair-dressed-casually-looking-with-satisfaction.jpg",
    },
  ],
  agendaTextAs: "Agenda",
  agendaIntro:
    "A stellar roster of design and product leaders to share their journeys and experiences with the community.",
});

// Participate data
const participate = ref({
  participateMethod: "get tickets",
  participateDetails:
    "Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.",
  paricipateBtnText: "Get Started",
});
</script>

<style></style>
