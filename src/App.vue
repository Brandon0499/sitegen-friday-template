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
    <MainTitleSection> </MainTitleSection>
    <AboutSection></AboutSection>
    <MarketingSection></MarketingSection>
    <CompanyEvents></CompanyEvents>
    <CompanyMembers></CompanyMembers>
    <IndividualAgenda :singleAgendas="singleAgendas"></IndividualAgenda>
    <ParticipateSection></ParticipateSection>

    <Footer></Footer>
  </div>
</template>

<script setup>
import Navbar from "./components/NavbarSection/Navbar.vue";
import MainTitleSection from "./components/MainTitleSection/MainTitleSection.vue";
import AboutSection from "./components/AboutSection/AboutSection.vue";
import MarketingSection from "./components/MarketingSection/MarketingSection.vue";
import CompanyEvents from "./components/CompanyInfoSection/CompanyEvents.vue";
import CompanyMembers from "./components/CompanyInfoSection/CompanyMembers.vue";
import IndividualAgenda from "./components/CompanyInfoSection/IndividualAgenda.vue";
import ParticipateSection from "./components/ParticipateSection/ParticipateSection.vue";
import Footer from "./components/FooterSection/Footer.vue";

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

const singleAgendas = ref([
  {
    day: "Day 01",
    date: "July 30",
    agendaSchedules: ["9:00 AM", "9.30 AM"],
    agendaTitle: "Build an employer brand that attracts top performers",
    agendaSummary:
      "Nulla vitae elit libero, a pharetra augue. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Sed posuere consectetur est at lobortis. Aenean lacinia bibendum nulla sed consectetur.Test1",
    showHiddenDetails: false,
    peopleInCharge: [
      {
        imageURL:
          "/assets/61e5bb75ba3a7e25e50bd527_isolated-shot-joyful-blonde-young.jpg",
        name: "Jessica Walsh",
        position: "Chief Officer",
      },
      {
        imageURL:
          "/assets/61e5bb75ba3a7e25e50bd527_isolated-shot-joyful-blonde-young.jpg",
        name: "Jessica Walsh",
        position: "Chief Officer",
      },
      {
        imageURL:
          "/assets/61e5bb75ba3a7e25e50bd527_isolated-shot-joyful-blonde-young.jpg",
        name: "Jessica Walsh",
        position: "Chief Officer",
      },
    ],
  },
  {
    day: "Day 02",
    date: "July 31",
    agendaSchedules: ["9:00 AM", "9.30 AM"],
    agendaTitle: "Build an employer brand that attracts top performers",
    agendaSummary:
      "Nulla vitae elit libero, a pharetra augue. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Sed posuere consectetur est at lobortis. Aenean lacinia bibendum nulla sed consectetur.Test2",
    showHiddenDetails: false,
    peopleInCharge: [
      {
        imageURL:
          "/assets/61e5bb75ba3a7e25e50bd527_isolated-shot-joyful-blonde-young.jpg",
        name: "Jessica Walsh",
        position: "Chief Officer",
      },
      {
        imageURL:
          "/assets/61e5bb75ba3a7e25e50bd527_isolated-shot-joyful-blonde-young.jpg",
        name: "Jessica Walsh",
        position: "Chief Officer",
      },
      {
        imageURL:
          "/assets/61e5bb75ba3a7e25e50bd527_isolated-shot-joyful-blonde-young.jpg",
        name: "Jessica Walsh",
        position: "Chief Officer",
      },
    ],
  },
]);
</script>

<style></style>
