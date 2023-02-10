<template>
  <div class="subscribe">
    <div class="subscribe-content">
      <h3 class="subscribe-title">Lorem ipsum, dolor sit ame</h3>
      <span class="subscribe-description"
        >Lorem ipsum dolor sit amet consectetur adipisicing elit. Hic tenetur
        quae corrupti excepturi animi consequuntur amet aliquam atque
        tempore.</span
      >
      <div class="subscribe-checks">
        <div class="subscribe-check">
          <img src="/svg/check.svg" class="subscribe-check__img" alt="" />
          <div class="subscribe-check__name">Lorem, ipsum.</div>
        </div>
        <div class="subscribe-check">
          <img src="/svg/check.svg" class="subscribe-check__img" alt="" />
          <div class="subscribe-check__name">Lorem, ipsum2.</div>
        </div>
        <div class="subscribe-check">
          <!-- svg -->
          <svg
            width="30px"
            height="30px"
            class="subscribe-check__svg"
            viewBox="0 0 24 24"
            version="1.1"
            xmlns="http://www.w3.org/2000/svg"
            xmlns:xlink="http://www.w3.org/1999/xlink"
          >
            <!-- Uploaded to: SVG Repo, www.svgrepo.com, Generator: SVG Repo Mixer Tools -->
            <title>ic_fluent_checkbox_unchecked_24_regular</title>
            <desc>Created with Sketch.</desc>
            <g
              id="🔍-Product-Icons"
              stroke="none"
              stroke-width="1"
              fill="none"
              fill-rule="evenodd"
            >
              <g
                id="ic_fluent_checkbox_unchecked_24_regular"
                fill="#212121"
                fill-rule="nonzero"
              >
                <path
                  d="M5.75,3 L18.25,3 C19.7687831,3 21,4.23121694 21,5.75 L21,18.25 C21,19.7687831 19.7687831,21 18.25,21 L5.75,21 C4.23121694,21 3,19.7687831 3,18.25 L3,5.75 C3,4.23121694 4.23121694,3 5.75,3 Z M5.75,4.5 C5.05964406,4.5 4.5,5.05964406 4.5,5.75 L4.5,18.25 C4.5,18.9403559 5.05964406,19.5 5.75,19.5 L18.25,19.5 C18.9403559,19.5 19.5,18.9403559 19.5,18.25 L19.5,5.75 C19.5,5.05964406 18.9403559,4.5 18.25,4.5 L5.75,4.5 Z"
                  id="🎨Color"
                ></path>
              </g>
            </g>
          </svg>
          <!-- svg -->
          <div class="subscribe-check__name">Lorem, ipsum3.</div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.subscribe {
  background: no-repeat center/cover url(/img/subscribe-background.jpg);
  padding: 97px 0 86px 0;
  &-content {
    max-width: 500px;
    margin: auto;
    text-align: center;
    color: #fff;
  }
  &-title {
    display: block;
    margin: 0 0 12px 0;
    font-weight: 400;
    font-family: var(--clash);
  }
  &-description {
    display: block;
    font-size: 18px;
  }
  &-checks {
    display: flex;
    justify-self: center;
  }
  &-check {
    display: flex;
    justify-content: center;
    &:nth-child(2) {
      margin: 0 36px;
    }
    &__icon {
      margin-right: 9px;
    }
    &__svg{
      fill: #fff;
    }
  }
}
</style>
