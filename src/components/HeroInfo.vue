<template>
  <div :style="{ backgroundColor: background }" class="hero-info">
    <div class="hero-info-text">
      <h2 class="hero-info-title" :style="{ color: colorTitle }">
        {{ title }}
      </h2>
      <span class="hero-info-description" :style="{ color: colorDescription }">
        {{ description }}
      </span>
    </div>
    <uiButton type="link" to="/" background="rgba(118, 118, 118, 0.15)">Lorem, ipsum.</uiButton>
    <!-- <a :style="{color:colorLink}" :href="link" class="hero-info-link">Lorem, ipsum.</a> -->
  </div>
</template>

<script setup>
import uiButton from '@/components/UI/Button.vue'
const props = defineProps({
  title: {
    type: String,
    required: false,
  },
  description: {
    type: String,
    required: false,
  },
  link: {
    type: String,
    required: false,
  },
  colorTitle: {
    type: String,
    default: "#5b5676;",
  },
  colorLink: {
    type: String,
    default: "#22202e",
  },
  colorDescription: {
    type: String,
    default: "#5b5676;",
  },
  background: {
    type: String,
    default: "#fff;",
  },
});
</script>

<style lang="scss" scoped>

.hero {
  &-info {
    max-width: 630px;
    padding: 50px 55px;
    min-height: 444px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    &-title {
      font-family: var(--clash);
      font-weight: 400;
      line-height: 1.5;
      margin: 0 0 20px 0;
    }
    &-description {
      font-size: 18px;
    }
  }
}
</style>
