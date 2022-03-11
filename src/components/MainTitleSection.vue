<template>
  <div class="section titles bg-red wf-section">
    <div class="container header w-container">
      <div class="w-layout-grid main-grid no-gap">
        <div
          id="w-node-f16383f7-a435-9fbd-d177-bd0fbd8c4c1c-0e305478"
          class="content-wrapper inner-padding-small"
        >
          <img
            :src="mainTitle.emojiURL"
            loading="lazy"
            width="206"
            alt=""
            class="image-smile"
          />
        </div>
        <div
          id="w-node-_457eb3c8-9b36-effc-ee78-fda56a38a58f-0e305478"
          class="overflow"
        >
          <div class="xlarge">{{ mainTitle.companyFirstName }}</div>
        </div>
        <div
          id="w-node-d0a5ca32-c852-da7c-b576-7f40495022cb-0e305478"
          class="content-wrapper flex-horizontal"
        >
          <div class="overflow-wrapper">
            <div class="overflow-wrapper flex">
              <div
                class="hero-flex-ticker"
                style="
                  transform: translate3d(-39.408%, 0px, 0px) scale3d(1, 1, 1)
                    rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
                  transform-style: preserve-3d;
                  will-change: transform;
                "
              >
                <div class="heading-regular uppercase">
                  the design event of the year
                </div>
                <div class="divider-bullet ticker"></div>
                <div class="heading-regular uppercase">#FFW 2022</div>
                <div class="divider-bullet ticker"></div>
                <div class="heading-regular uppercase">grab a spot</div>
                <div class="divider-bullet ticker"></div>
              </div>
              <div
                class="hero-flex-ticker"
                style="
                  transform: translate3d(-39.408%, 0px, 0px) scale3d(1, 1, 1)
                    rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
                  transform-style: preserve-3d;
                  will-change: transform;
                "
              >
                <div class="heading-regular uppercase">
                  the design event of the year
                </div>
                <div class="divider-bullet ticker"></div>
                <div class="heading-regular uppercase">#FFW 2022</div>
                <div class="divider-bullet ticker"></div>
                <div class="heading-regular uppercase">grab a spot</div>
                <div class="divider-bullet ticker"></div>
              </div>
              <div
                class="hero-flex-ticker"
                style="
                  transform: translate3d(-39.408%, 0px, 0px) scale3d(1, 1, 1)
                    rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
                  transform-style: preserve-3d;
                  will-change: transform;
                "
              >
                <div class="heading-regular uppercase">
                  the design event of the year
                </div>
                <div class="divider-bullet ticker"></div>
                <div class="heading-regular uppercase">#FFW 2022</div>
                <div class="divider-bullet ticker"></div>
                <div class="heading-regular uppercase">grab a spot</div>
                <div class="divider-bullet ticker"></div>
              </div>
            </div>
          </div>
          <div class="xlarge">{{ mainTitle.eventActivity }}</div>
        </div>
      </div>
      <div class="wrapper-heading inner-padding-small">
        <div class="w-layout-grid grid-buttons">
          <div id="w-node-acbeed1e-14e6-2f5d-f965-c0dfd171fa89-0e305478">
            <div
              data-w-id="f22dbb03-ea9e-a94b-045a-7963939b43b2"
              class="main-button-wrap"
            >
              <a
                id="w-node-f22dbb03-ea9e-a94b-045a-7963939b43b3-939b43b2"
                href="https://webflow.com/templates/html/friday-conference-website-template"
                target="_blank"
                class="button w-inline-block"
                style="
                  transform: translate3d(0px, 0px, 0px) scale3d(1, 1, 1)
                    rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
                  transform-style: preserve-3d;
                "
                ><div class="m-button-label">
                  <div
                    class="circular-arrow"
                    style="background-color: rgb(241, 173, 46)"
                  >
                    <img
                      src="/assets/61e5bb75ba3a7ec9880bd403_cta-arrow-white.svg"
                      loading="lazy"
                      alt=""
                      class="icon-arrow"
                    />
                  </div>
                  <div class="label-button" style="color: rgb(255, 255, 255)">
                    {{ mainTitle.joinButtonText }}
                  </div>
                </div>
                <div
                  class="m-button-hover"
                  style="
                    transform: translate3d(-102%, 0px, 0px) scale3d(1, 1, 1)
                      rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
                    transform-style: preserve-3d;
                  "
                ></div
              ></a>
              <div class="m-button-shadow" style="display: none"></div>
            </div>
          </div>
          <a
            id="w-node-_786cc278-92ec-6bcd-270f-eeb81f660a90-0e305478"
            href="https://friday-template.webflow.io/landing/01#"
            class="button inline w-inline-block"
            ><div>{{ mainTitle.learnMoreText }}</div>
            <div
              class="outline-hover"
              style="
                transform: translate3d(-102%, 0px, 0px) scale3d(1, 1, 1)
                  rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
                transform-style: preserve-3d;
              "
            ></div
          ></a>
        </div>
      </div>
    </div>
    <Promotions>
      <slot name="test"></slot>
    </Promotions>
  </div>
</template>

<script setup>
const props = defineProps({
  mainTitle: {
    type: Object,
    required: true,
  },
});
</script>

<style></style>
