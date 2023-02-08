<template>
  <div class="container">
    <Header />
    <Heromain />
    <AboutBrand />
    <Products />
    <Started />
  </div>
</template>

<script setup>
import Products from "./components/ProductsBlock.vue";
import Heromain from "./components/HeroMain.vue";
import Header from "./components/Layout/Header.vue";
import AboutBrand from "./components/AboutBrand.vue";
import Started from "./components/Started.vue";
</script>

<style lang="scss">
@import url("https://fonts.cdnfonts.com/css/satoshi");
@import url("https://fonts.cdnfonts.com/css/clash-display");
* {
  box-sizing: border-box;
  font-weight: 400;
}
body {
  font-family: "Satoshi", sans-serif;
  margin: 0;
  padding: 0;
  font-size: 16px;
  color: #22202e;
}
img {
  max-width: 100%;
}
.container {
  max-width: 1440px;
  margin: auto;
}
</style>
