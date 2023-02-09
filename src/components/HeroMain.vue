<template>
  <div class="hero">
    <HeroInfo
    title="Lorem ipsum, dolor sit amet consectetur adipisicing."
    description="Lorem ipsum, dolor sit amet consectetur adipisicing elit. Facere maiores
        eveniet animi, magnam repellendus placeat." 
    link="#"
    colorLink="lightgray"
    background="#fff"/>
  </div>
</template>

<script setup>
import HeroInfo from "@/components/HeroInfo.vue";
</script>
<style lang="scss" scoped>
.hero {
  background: url("/img/main-hero.jpg");
  height: 704px;
  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  padding-right: 80px;
}
</style>
