<template>
  <div class="container padding-bottom-medium">
    <WavesSeparator></WavesSeparator>
    <div class="w-layout-grid main-grid">
      <div
        id="w-node-_1783bf35-b007-14db-9815-20711d5e0fab-0e305478"
        class="center-wrapper inner-padding-medium"
      >
        <h2 class="heading-large margin-bottom-xsmall">
          {{ companyInfo.agendaTextAs }}
        </h2>
        <p class="medium-paragraph">
          {{ companyInfo.agendaIntro }}
        </p>
      </div>
    </div>
    <IndividualAgenda :agendas="agendas"></IndividualAgenda>
  </div>
</template>

<script setup>
import { ref } from "@vue/reactivity";
import IndividualAgenda from "./IndividualAgenda.vue";

const agendas = ref({
  singleAgendas: [
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
  ],
});

const props = defineProps({
  companyInfo: {
    type: Object,
    required: true,
  },
});
</script>

<style></style>
