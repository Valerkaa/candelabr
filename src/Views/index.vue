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
  import Products from "@/components/ProductsBlock.vue";
  import Heromain from "@/components/HeroMain.vue";
  import Header from "@/components/Layout/Header.vue";
  import AboutBrand from "@/components/AboutBrand.vue";
  import Started from "@/components/Started.vue";
  </script>
  