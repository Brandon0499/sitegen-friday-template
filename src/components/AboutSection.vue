<template>
  <div class="section bg-color wf-section">
    <div class="container top-padding-large w-container">
      <div class="w-layout-grid main-grid padding-bottom-medium">
        <div
          id="w-node-_2b6e6bfb-df51-26f9-8670-bce9cb867456-0e305478"
          class="callout-wrapper padding-bottom-small"
        >
          <h1 class="heading-xlarge text-yellow margin-bottom-small">
            {{ about.companySlogan }}
          </h1>
          <p class="main-paragraph size-large text-white-opacity">
            {{ about.companySummary }}
          </p>
          <div class="flex">
            <div
              data-w-id="b4c2dd96-84ad-3220-d100-e3d8ca40b388"
              data-animation-type="lottie"
              data-src="https://assets.website-files.com/61e5bb75ba3a7e40020bd3b2/620a95bf9ede664b27335e16_shape1_pink.json"
              data-loop="1"
              data-direction="1"
              data-autoplay="1"
              data-is-ix2-target="0"
              data-renderer="svg"
              data-default-duration="3"
              data-duration="0"
              class="lottie-animation-2"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 139 34"
                width="139"
                height="34"
                preserveAspectRatio="xMidYMid meet"
                style="
                  width: 100%;
                  height: 100%;
                  transform: translate3d(0px, 0px, 0px);
                "
              >
                <defs>
                  <clippath id="__lottie_element_62">
                    <rect width="139" height="34" x="0" y="0"></rect>
                  </clippath>
                </defs>
                <g clip-path="url(#__lottie_element_62)">
                  <g
                    transform="matrix(1,0,0,1,38.61900329589844,-32.295997619628906)"
                    opacity="1"
                    style="display: block"
                  >
                    <g opacity="1" transform="matrix(1,0,0,1,0,0)">
                      <path
                        stroke-linecap="round"
                        stroke-linejoin="miter"
                        fill-opacity="0"
                        stroke-miterlimit="4"
                        stroke-dasharray=" 102 25"
                        stroke-dashoffset="30.233993530273438"
                        stroke="rgb(244,132,125)"
                        stroke-opacity="1"
                        stroke-width="8"
                        d=" M93.38200378417969,41.233001708984375 C77.86599731445312,41.233001708984375 77.86599731445312,55.14699935913086 62.349998474121094,55.14699935913086 C46.83399963378906,55.14699935913086 46.834999084472656,41.233001708984375 31.319000244140625,41.233001708984375 C15.803000450134277,41.233001708984375 15.803999900817871,55.14699935913086 0.2879999876022339,55.14699935913086 C-15.227999687194824,55.14699935913086 -15.22700023651123,41.233001708984375 -30.743000030517578,41.233001708984375"
                      ></path>
                    </g>
                  </g>
                </g>
              </svg>
            </div>
          </div>
        </div>

        <div
          id="w-node-_6341ee7c-c590-47e8-d3cc-5c75418cc276-0e305478"
          class="callout-wrapper"
        >
          <h2 class="heading-small">About {{ about.companyFullName }}</h2>
        </div>
      </div>
      <div class="statisticsWrapper">
        <div
          class="callout-box-wrapper statisticsSpace"
          v-for="statistic in about.statistics"
          :key="statistic.statisticFor"
        >
          <div class="value large text-yellow">
            {{ statistic.statisticNumbers }}
          </div>
          <h2 class="heading-small">{{ statistic.statisticFor }}</h2>
        </div>
      </div>
    </div>
    <div class="flex-scrolling" style="margin-top: 40px">
      <div
        class="w-layout-grid logo-grid-ticker"
        style="
          transform: translate3d(-69.963%, 0px, 0px) scale3d(1, 1, 1)
            rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
          transform-style: preserve-3d;
          will-change: transform;
        "
      >
        <div
          class="logo-wrap-ticker"
          v-for="sponsor in about.sponsors"
          :key="sponsor.sponsorImageURL"
        >
          <img
            :src="sponsor.sponsorImageURL"
            loading="lazy"
            alt=""
            class="company-logo"
          />
        </div>
      </div>
      <div
        class="w-layout-grid logo-grid-ticker"
        style="
          transform: translate3d(-69.963%, 0px, 0px) scale3d(1, 1, 1)
            rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
          transform-style: preserve-3d;
          will-change: transform;
        "
      >
        <div
          class="logo-wrap-ticker"
          v-for="sponsor in about.sponsors"
          :key="sponsor.sponsorImageURL"
        >
          <img
            :src="sponsor.sponsorImageURL"
            loading="lazy"
            alt=""
            class="company-logo"
          />
        </div>
      </div>
      <div
        class="w-layout-grid logo-grid-ticker"
        style="
          transform: translate3d(-69.963%, 0px, 0px) scale3d(1, 1, 1)
            rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
          transform-style: preserve-3d;
          will-change: transform;
        "
      >
        <div
          v-for="sponsor in about.sponsors"
          :key="sponsor.sponsorImageURL"
          class="logo-wrap-ticker"
        >
          <img
            :key="sponsor.sponsorImageURL"
            loading="lazy"
            alt=""
            class="company-logo"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  about: {
    type: Object,
    required: true,
  },
});
</script>

<style scoped>
.statisticsSpace {
  margin-bottom: 40px;
}
@media (min-width: 990px) {
  .statisticsWrapper {
    margin-left: 35%;
  }
}
</style>
