<template>
  <div class="hero-info">
    <div class="hero-info-text"
    :style="{backgroundColor:background}">
      <h2 class="hero-info-title"
      :style="{color:colorTitle}">
      {{ title}}
      </h2>
      <span class="hero-info-description"
      :style="{color:colorDescription}">
      {{ description }}
      </span>
    </div>
    <a :href="link" class="hero-info-link">Lorem, ipsum.</a>
  </div>
</template>

<script setup>
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
    default: '',
  },
  colorDescription: {
    type: String,
    default: '#5b5676;',
  },
  background: {
    type: String,
    default: '#fff;',
  },
  
});
</script>

<style lang="scss" scoped>
@import url("https://fonts.cdnfonts.com/css/clash-display");
.hero {
  &-info {
    &-title {
      font-family: "Clash Display", sans-serif;
      font-weight: 400;
      line-height: 1.5;
      margin: 0 0 20px 0;
    }
    &-description {
      color: #5b5676;
      font-size: 18px;
    }
    &-link {
      color: #2a254b;
      text-decoration: none;
      &:hover {
        text-decoration: underline;
      }
    }
  }
}
</style>
