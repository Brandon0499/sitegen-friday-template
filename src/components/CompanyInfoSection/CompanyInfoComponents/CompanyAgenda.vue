<template>
  <div class="section bg-dark-gray wf-section">
    <div class="container padding-bottom-medium">
      <WavesSeparator></WavesSeparator>
      <div class="w-layout-grid main-grid">
        <div
          id="w-node-_1783bf35-b007-14db-9815-20711d5e0fab-0e305478"
          class="center-wrapper inner-padding-medium"
        >
          <h2 class="heading-large margin-bottom-xsmall">
            {{ props.agendaTextAs }}
          </h2>
          <p class="medium-paragraph">
            {{ props.agendaIntro }}
          </p>
        </div>
      </div>
      <IndividualAgenda :agendas="agendas"></IndividualAgenda>
    </div>
  </div>
</template>

<script setup>
import { ref } from "@vue/reactivity";
import IndividualAgenda from "./IndividualAgenda.vue";

const props = defineProps({
  agendaTextAs: {
    type: String,
    default: "Agenda",
  },
  agendaIntro: {
    type: String,
    default:
      "A stellar roster of design and product leaders to share their journeys and experiences with the community.",
  },
});
</script>

<style scoped>
.agendaPadding {
  padding: 30px;
}
</style>
