<template>
  <div class="container padding-bottom-medium">
    <div class="container">
      <div class="w-layout-grid main-grid">
        <div
          id="w-node-_6e7598f0-4ae8-b765-38bc-ef4f35557c1a-0e305478"
          class="center-wrapper inner-padding-medium"
        >
          <h2 class="heading-large margin-bottom-xsmall">
            {{ companyInfo.memberTextAs }}
          </h2>
          <p class="medium-paragraph">
            {{ companyInfo.membersIntro }}
          </p>
        </div>
      </div>
    </div>
    <div class="w-dyn-list">
      <div role="list" class="collection-list-col w-dyn-items">
        <div
          id="w-node-_6e7598f0-4ae8-b765-38bc-ef4f35557c20-0e305478"
          role="listitem"
          class="collection-item w-dyn-item"
          v-for="member in companyInfo.members"
          :key="member.memberName"
        >
          <a
            data-w-id="6e7598f0-4ae8-b765-38bc-ef4f35557c21"
            :href="member.memberProfileLink"
            class="link-block w-inline-block"
            ><div
              data-w-id="6e7598f0-4ae8-b765-38bc-ef4f35557c23"
              style="
                background-color: rgb(40, 74, 168);
                transform: translate3d(0px, 102%, 0px) scale3d(1, 1, 1)
                  rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
                transform-style: preserve-3d;
              "
              class="box-speakers"
            >
              <div class="overflow">
                <div
                  class="speaker-ticker-wrapper left"
                  style="
                    transform: translate3d(0px, 100%, 0px) scale3d(1, 1, 1)
                      rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
                    transform-style: preserve-3d;
                  "
                >
                  <div
                    class="s-ticker-flex"
                    style="
                      transform: translate3d(-38.47%, 0px, 0px) scale3d(1, 1, 1)
                        rotateX(0deg) rotateY(0deg) rotateZ(0deg)
                        skew(0deg, 0deg);
                      transform-style: preserve-3d;
                      will-change: transform;
                    "
                  >
                    <div
                      style="color: hsla(208, 95.22%, 68.37%, 1)"
                      class="heading-large no-wrap"
                    >
                      {{ member.memberName }}
                    </div>
                    <div
                      style="background-color: hsla(208, 95.22%, 68.37%, 1)"
                      class="dot-divider"
                    ></div>
                  </div>
                  <div
                    class="s-ticker-flex"
                    style="
                      transform: translate3d(-38.47%, 0px, 0px) scale3d(1, 1, 1)
                        rotateX(0deg) rotateY(0deg) rotateZ(0deg)
                        skew(0deg, 0deg);
                      transform-style: preserve-3d;
                      will-change: transform;
                    "
                  >
                    <div
                      style="color: hsla(208, 95.22%, 68.37%, 1)"
                      class="heading-large no-wrap"
                    >
                      {{ member.memberName }}
                    </div>
                    <div
                      style="background-color: hsla(208, 95.22%, 68.37%, 1)"
                      class="dot-divider"
                    ></div>
                  </div>
                  <div
                    class="s-ticker-flex"
                    style="
                      transform: translate3d(-38.47%, 0px, 0px) scale3d(1, 1, 1)
                        rotateX(0deg) rotateY(0deg) rotateZ(0deg)
                        skew(0deg, 0deg);
                      transform-style: preserve-3d;
                      will-change: transform;
                    "
                  >
                    <div
                      style="color: hsla(208, 95.22%, 68.37%, 1)"
                      class="heading-large no-wrap"
                    >
                      {{ member.memberName }}
                    </div>
                    <div
                      style="background-color: hsla(208, 95.22%, 68.37%, 1)"
                      class="dot-divider"
                    ></div>
                  </div>
                </div>
              </div>
              <div class="overflow">
                <div
                  data-w-id="6e7598f0-4ae8-b765-38bc-ef4f35557c30"
                  class="speaker-ticker-wrapper"
                  style="
                    transform: translate3d(0px, 100%, 0px) scale3d(1, 1, 1)
                      rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
                    transform-style: preserve-3d;
                  "
                >
                  <div
                    style="
                      transform: translate3d(-61.53%, 0px, 0px) scale3d(1, 1, 1)
                        rotateX(0deg) rotateY(0deg) rotateZ(0deg)
                        skew(0deg, 0deg);
                      transform-style: preserve-3d;
                      will-change: transform;
                    "
                    class="s-ticker-flex right"
                  >
                    <div
                      style="color: hsla(208, 95.22%, 68.37%, 1)"
                      class="heading-large no-wrap"
                    >
                      {{ member.memberName }}
                    </div>
                    <div
                      style="background-color: hsla(208, 95.22%, 68.37%, 1)"
                      class="dot-divider"
                    ></div>
                  </div>
                  <div
                    style="
                      transform: translate3d(-61.53%, 0px, 0px) scale3d(1, 1, 1)
                        rotateX(0deg) rotateY(0deg) rotateZ(0deg)
                        skew(0deg, 0deg);
                      transform-style: preserve-3d;
                      will-change: transform;
                    "
                    class="s-ticker-flex right"
                  >
                    <div
                      style="color: hsla(208, 95.22%, 68.37%, 1)"
                      class="heading-large no-wrap"
                    >
                      {{ member.memberName }}
                    </div>
                    <div
                      style="background-color: hsla(208, 95.22%, 68.37%, 1)"
                      class="dot-divider"
                    ></div>
                  </div>
                  <div
                    style="
                      transform: translate3d(-61.53%, 0px, 0px) scale3d(1, 1, 1)
                        rotateX(0deg) rotateY(0deg) rotateZ(0deg)
                        skew(0deg, 0deg);
                      transform-style: preserve-3d;
                      will-change: transform;
                    "
                    class="s-ticker-flex right"
                  >
                    <div
                      style="color: hsla(208, 95.22%, 68.37%, 1)"
                      class="heading-large no-wrap"
                    >
                      {{ member.memberName }}
                    </div>
                    <div
                      style="background-color: hsla(208, 95.22%, 68.37%, 1)"
                      class="dot-divider"
                    ></div>
                  </div>
                </div>
              </div>
              <div class="overflow">
                <div
                  class="speaker-ticker-wrapper left"
                  style="
                    transform: translate3d(0px, 100%, 0px) scale3d(1, 1, 1)
                      rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
                    transform-style: preserve-3d;
                  "
                >
                  <div
                    class="s-ticker-flex"
                    style="
                      transform: translate3d(-38.47%, 0px, 0px) scale3d(1, 1, 1)
                        rotateX(0deg) rotateY(0deg) rotateZ(0deg)
                        skew(0deg, 0deg);
                      transform-style: preserve-3d;
                      will-change: transform;
                    "
                  >
                    <div
                      style="color: hsla(208, 95.22%, 68.37%, 1)"
                      class="heading-large no-wrap"
                    >
                      {{ member.memberName }}
                    </div>
                    <div
                      style="background-color: hsla(208, 95.22%, 68.37%, 1)"
                      class="dot-divider"
                    ></div>
                  </div>
                  <div
                    class="s-ticker-flex"
                    style="
                      transform: translate3d(-38.47%, 0px, 0px) scale3d(1, 1, 1)
                        rotateX(0deg) rotateY(0deg) rotateZ(0deg)
                        skew(0deg, 0deg);
                      transform-style: preserve-3d;
                      will-change: transform;
                    "
                  >
                    <div
                      style="color: hsla(208, 95.22%, 68.37%, 1)"
                      class="heading-large no-wrap"
                    >
                      {{ member.memberName }}
                    </div>
                    <div
                      style="background-color: hsla(208, 95.22%, 68.37%, 1)"
                      class="dot-divider"
                    ></div>
                  </div>
                  <div
                    class="s-ticker-flex"
                    style="
                      transform: translate3d(-38.47%, 0px, 0px) scale3d(1, 1, 1)
                        rotateX(0deg) rotateY(0deg) rotateZ(0deg)
                        skew(0deg, 0deg);
                      transform-style: preserve-3d;
                      will-change: transform;
                    "
                  >
                    <div
                      style="color: hsla(208, 95.22%, 68.37%, 1)"
                      class="heading-large no-wrap"
                    >
                      {{ member.memberName }}
                    </div>
                    <div
                      style="background-color: hsla(208, 95.22%, 68.37%, 1)"
                      class="dot-divider"
                    ></div>
                  </div>
                </div>
              </div>
              <div class="overflow">
                <div
                  data-w-id="6e7598f0-4ae8-b765-38bc-ef4f35557c46"
                  class="speaker-ticker-wrapper"
                  style="
                    transform: translate3d(0px, 100%, 0px) scale3d(1, 1, 1)
                      rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
                    transform-style: preserve-3d;
                  "
                >
                  <div
                    style="
                      transform: translate3d(-61.53%, 0px, 0px) scale3d(1, 1, 1)
                        rotateX(0deg) rotateY(0deg) rotateZ(0deg)
                        skew(0deg, 0deg);
                      transform-style: preserve-3d;
                      will-change: transform;
                    "
                    class="s-ticker-flex right"
                  >
                    <div
                      style="color: hsla(208, 95.22%, 68.37%, 1)"
                      class="heading-large no-wrap"
                    >
                      {{ member.memberName }}
                    </div>
                    <div
                      style="background-color: hsla(208, 95.22%, 68.37%, 1)"
                      class="dot-divider"
                    ></div>
                  </div>
                  <div
                    style="
                      transform: translate3d(-61.53%, 0px, 0px) scale3d(1, 1, 1)
                        rotateX(0deg) rotateY(0deg) rotateZ(0deg)
                        skew(0deg, 0deg);
                      transform-style: preserve-3d;
                      will-change: transform;
                    "
                    class="s-ticker-flex right"
                  >
                    <div
                      style="color: hsla(208, 95.22%, 68.37%, 1)"
                      class="heading-large no-wrap"
                    >
                      {{ member.memberName }}
                    </div>
                    <div
                      style="background-color: hsla(208, 95.22%, 68.37%, 1)"
                      class="dot-divider"
                    ></div>
                  </div>
                  <div
                    style="
                      transform: translate3d(-61.53%, 0px, 0px) scale3d(1, 1, 1)
                        rotateX(0deg) rotateY(0deg) rotateZ(0deg)
                        skew(0deg, 0deg);
                      transform-style: preserve-3d;
                      will-change: transform;
                    "
                    class="s-ticker-flex right"
                  >
                    <div
                      style="color: hsla(208, 95.22%, 68.37%, 1)"
                      class="heading-large no-wrap"
                    >
                      {{ member.memberName }}
                    </div>
                    <div
                      style="background-color: hsla(208, 95.22%, 68.37%, 1)"
                      class="dot-divider"
                    ></div>
                  </div>
                </div>
              </div>
            </div>
            <img
              :src="member.memberImageURL"
              loading="lazy"
              alt=""
              class="cover-image relative"
          /></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  companyInfo: {
    type: Object,
    required: true,
  },
});
</script>

<style></style>
