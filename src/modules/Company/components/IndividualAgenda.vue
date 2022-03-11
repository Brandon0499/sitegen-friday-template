<template>
  <div
    class="rounded-box"
    v-for="singleAgenda in agendas.singleAgendas"
    :key="singleAgenda.day"
  >
    <div class="w-layout-grid main-grid">
      <div id="w-node-_54adcaaa-0454-a003-4d72-1777ed4c39cb-0e305478">
        <div class="date-spot">
          <div class="heading-small">{{ singleAgenda.day }}</div>
          <div class="heading-small">{{ singleAgenda.date }}</div>
        </div>
      </div>
      <div id="w-node-_54adcaaa-0454-a003-4d72-1777ed4c39d0-0e305478">
        <div class="faq-wrapper divider">
          <a
            href="#hello"
            class="faq-link w-inline-block"
            @click="toggleHiddenDetails(singleAgenda)"
          >
            <div>
              <div class="timeline-wrapper">
                <div
                  class="text-date bg-color"
                  v-for="agendaSchedule in singleAgenda.agendaSchedules"
                  :key="agendaSchedule"
                >
                  {{ agendaSchedule }}
                </div>
              </div>
              <div class="heading-medium text-white margin-bottom-xsmall">
                {{ singleAgenda.agendaTitle }}
              </div>
            </div>
            <div
              class="faq-icon"
              :class="{
                rotate: singleAgenda.showHiddenDetails,
                rotateOpposite: !singleAgenda.showHiddenDetails,
              }"
            >
              <img
                loading="lazy"
                src="/assets/61e5bb75ba3a7e42260bd3f0_icon-plus.svg"
                alt=""
                class="plus-icon"
              />
            </div>
          </a>
          <div
            class="faq-container"
            :class="{
              showHiddenDetails: singleAgenda.showHiddenDetails,
              hideHiddenDetails: !singleAgenda.showHiddenDetails,
            }"
          >
            <p class="medium-paragraph">
              {{ singleAgenda.agendaSummary }}
            </p>
            <div class="content-wrapper inner-padding-micro">
              <div
                class="w-layout-grid auto-grid profile"
                v-for="personInCharge in singleAgenda.peopleInCharge"
                :key="personInCharge.imageURL"
              >
                <div class="square-profile">
                  <img
                    sizes="100vw"
                    srcset="
                      https://assets.website-files.com/61e5bb75ba3a7e40020bd3b2/61e5bb75ba3a7e25e50bd527_isolated-shot-joyful-blonde-young-p-500.jpeg  500w,
                      https://assets.website-files.com/61e5bb75ba3a7e40020bd3b2/61e5bb75ba3a7e25e50bd527_isolated-shot-joyful-blonde-young-p-800.jpeg  800w,
                      https://assets.website-files.com/61e5bb75ba3a7e40020bd3b2/61e5bb75ba3a7e25e50bd527_isolated-shot-joyful-blonde-young.jpg        1200w
                    "
                    :src="personInCharge.imageURL"
                    loading="lazy"
                    alt=""
                    class="cover-image"
                  />
                </div>
                <div>
                  <div class="main-paragraph bold">
                    {{ personInCharge.name }}
                  </div>
                  <div class="main-paragraph size-small text-white-opacity">
                    {{ personInCharge.position }}
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  agendas: {
    type: Object,
    required: true,
  },
});

function toggleHiddenDetails(agenda) {
  agenda.showHiddenDetails = !agenda.showHiddenDetails;
}
</script>

<style scoped>
.showHiddenDetails {
  display: block;
}

.hideHiddenDetails {
  display: none;
}

.rotate {
  transform: rotate(45deg);
  transition-duration: 0.3s;
  transition-timing-function: ease-in-out;
}

.rotateOpposite {
  transform: rotate(0deg);
  transition-duration: 0.3s;
  transition-timing-function: ease-in-out;
}
</style>
