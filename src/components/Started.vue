<template>
    <div class="started">
        <HeroInfo
        title="Lorem ipsum dolor sit, amet consectetur adipisicing elit. Aspernatur quo impedit accusamus id, repudiandae qui."
        description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum labore necessitatibus, voluptate omnis iure porro sit! Minus reiciendis dolor repudiandae labore impedit consequatur. Repellat, sapiente?"
        link="#"
        colorTitle="#fff"
        colorDescription="#fff"
        background="var(--purple)"
        colorLink="secondary"/>
        <img src="/img/started-img.jpg" alt="">
    </div>
</template>
<script setup>
import HeroInfo from '@/components/HeroInfo.vue';
</script>


<style lang="scss" scoped>
.started{
    padding: 0 80px;
    margin-bottom: 60px;
    display: grid;
    grid-template-columns: repeat(2 , 1fr);
    column-gap: 16px;
}
</style>