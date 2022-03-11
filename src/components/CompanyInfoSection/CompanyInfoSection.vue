<template>
  <div class="section bg-dark-gray wf-section">
    <div class="container padding-top-large w-container">
      <div class="w-layout-grid main-grid">
        <a
          id="w-node-_12ff7464-3378-7f39-ebe9-0837a7ccdcfa-0e305478"
          href="https://friday-template.webflow.io/landing/01#"
          class="content-wrapper cards w-inline-block"
          ><div class="w-layout-grid grid-card">
            <div class="imgContainer">
              <img
                src="https://www.museumnext.com/wp-content/uploads/2017/06/Designing-an-Exhibition-1.jpg"
                alt=""
                class="eventImage"
              />
            </div>
            <div
              id="w-node-_12ff7464-3378-7f39-ebe9-0837a7ccdcfe-0e305478"
              class="inner-card-content"
            >
              <h2 class="heading-large margin-bottom-xsmall">Exhibitions</h2>
              <p class="main-paragraph text-white-opacity-strong">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Suspendisse varius enim in eros elementum tristique.
              </p>
            </div>
          </div></a
        ><a
          id="w-node-_12ff7464-3378-7f39-ebe9-0837a7ccdd03-0e305478"
          href="https://friday-template.webflow.io/landing/01#"
          class="content-wrapper cards w-inline-block"
          ><div class="w-layout-grid grid-card">
            <div class="center-flex-wrapper-device square bg-yellow">
              <div
                data-w-id="6f0571eb-a6b0-3ff7-15e8-9795c501087b"
                data-animation-type="lottie"
                data-src="https://assets.website-files.com/61e5bb75ba3a7e40020bd3b2/620a965c4bcc42041eedfcc8_shape%202%20blue.json"
                data-loop="1"
                data-direction="1"
                data-autoplay="1"
                data-is-ix2-target="0"
                data-renderer="svg"
                data-default-duration="3"
                data-duration="0"
                class="lottie-animation-2 page"
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 124 125"
                  width="124"
                  height="125"
                  preserveAspectRatio="xMidYMid meet"
                  style="
                    width: 100%;
                    height: 100%;
                    transform: translate3d(0px, 0px, 0px);
                  "
                >
                  <defs>
                    <clippath id="__lottie_element_93">
                      <rect width="124" height="125" x="0" y="0"></rect>
                    </clippath>
                  </defs>
                  <g clip-path="url(#__lottie_element_93)">
                    <g
                      transform="matrix(0.47603753209114075,0.012049095705151558,-0.012049095705151558,0.47603753209114075,203.0300750732422,-42.79827117919922)"
                      opacity="1"
                      style="display: block"
                    >
                      <g
                        opacity="1"
                        transform="matrix(0.8073499798774719,0,0,0.8073499798774719,-290.5,227.5)"
                      >
                        <path
                          stroke-linecap="butt"
                          stroke-linejoin="miter"
                          fill-opacity="0"
                          stroke-miterlimit="4"
                          stroke="rgb(118,106,253)"
                          stroke-opacity="1"
                          stroke-width="101"
                          d=" M0,105 C0,105 0,105 0,105 C-57.949501037597656,105 -105,57.949501037597656 -105,0 C-105,0 -105,0 -105,0 C-105,-57.949501037597656 -57.949501037597656,-105 0,-105 C0,-105 0,-105 0,-105"
                        ></path>
                      </g>
                    </g>
                    <g
                      transform="matrix(0.9993723630905151,0.03539327159523964,-0.03539327159523964,0.9993723630905151,61.98735046386719,62.499847412109375)"
                      opacity="1"
                      style="display: block"
                    >
                      <g opacity="1" transform="matrix(1,0,0,1,-18.5,-37.25)">
                        <path
                          fill="rgb(167,187,255)"
                          fill-opacity="1"
                          d=" M0,-13.5 C7.450650215148926,-13.5 13.5,-7.450650215148926 13.5,0 C13.5,7.450650215148926 7.450650215148926,13.5 0,13.5 C-7.450650215148926,13.5 -13.5,7.450650215148926 -13.5,0 C-13.5,-7.450650215148926 -7.450650215148926,-13.5 0,-13.5z"
                        ></path>
                        <path
                          stroke-linecap="butt"
                          stroke-linejoin="miter"
                          fill-opacity="0"
                          stroke-miterlimit="4"
                          stroke="rgb(219,112,229)"
                          stroke-opacity="1"
                          stroke-width="0"
                          d=" M0,-13.5 C7.450650215148926,-13.5 13.5,-7.450650215148926 13.5,0 C13.5,7.450650215148926 7.450650215148926,13.5 0,13.5 C-7.450650215148926,13.5 -13.5,7.450650215148926 -13.5,0 C-13.5,-7.450650215148926 -7.450650215148926,-13.5 0,-13.5z"
                        ></path>
                      </g>
                    </g>
                  </g>
                </svg>
              </div>
            </div>
            <div
              id="w-node-_12ff7464-3378-7f39-ebe9-0837a7ccdd07-0e305478"
              class="inner-card-content"
            >
              <h2 class="heading-large margin-bottom-xsmall">workshops</h2>
              <p class="main-paragraph text-white-opacity-strong">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Suspendisse varius enim in eros elementum tristique.
              </p>
            </div>
          </div></a
        >
      </div>
      <!-- <WavesSeparator></WavesSeparator> -->
    </div>

    <!-- <WavesSeparator></WavesSeparator> -->
    <CompanyMembers :companyInfo="companyInfo"></CompanyMembers>
    <WavesSeparator></WavesSeparator>
    <CompanyAgenda :companyInfo="companyInfo"></CompanyAgenda>
  </div>
</template>

<script setup>
import WavesSeparator from "../WavesSeparator.vue";
import CompanyMembers from "./CompanyInfoComponents/CompanyMembers.vue";
import CompanyAgenda from "./CompanyInfoComponents/CompanyAgenda.vue";

const props = defineProps({
  companyInfo: {
    type: Object,
    required: true,
  },
});
</script>

<style scoped>
.imgContainer {
  height: 40em;
  outline: 1px solid white;
  object-fit: fill;
  border-radius: 35px;
  overflow: hidden;
}

.eventImage {
  height: 40em;
  object-fit: cover;
}
</style>
