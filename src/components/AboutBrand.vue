<template>
  <div class="about-brand">
    <h3 class="about-brand-title">Lorem ipsum dolor sit amet.</h3>
  <div class="about-brand-elements">
    <div class="about-brand-element" 
    v-for="(element, i) in aboutBrands" 
    :key="i">
        <img class="about-brand-element__image"
        :src="element.img"
        :alt="element.title"
       >
        <h4 class="about-brand-element__title">{{ element.title }}</h4>
        <span class="about-brand-element__description">{{ element.description }}</span>
    </div>
  </div>
</div>
</template>

<script setup>
import { ref } from 'vue';
const aboutBrands = [
    {  
    img:'/svg/about-brand-1.svg',
    title:' Lorem ipsum',
    description:'Lorem ipsum dolor sit amet consectetur.'
    },
    {  
    img:'/svg/about-brand-2.svg',
    title:' Lorem ipsum',
    description:'Lorem ipsum dolor sit amet consectetur.'
    },
    {  
    img:'/svg/about-brand-3.svg',
    title:' Lorem ipsum',
    description:'Lorem ipsum dolor sit amet consectetur.'
    },
    {  
    img:'/svg/about-brand-4.svg',
    title:' Lorem ipsum',
    description:'Lorem ipsum dolor sit amet consectetur.'
    }
]

</script>

<style lang="scss" scoped>
.about-brand {
  padding: 80px 0 130px 0;
  &-title {
    text-align: center;
    font-size: 24px;
    color: var(--purple);
    margin: 0 0 84px 0;
  }
  &-elements{
    
    display: grid;
    grid-template-columns: repeat(4, 210px);
    justify-content: space-between;
  }
  &-element{
    color: var(--purple);
    &__image{
        display: block;
        margin-bottom: 12px;
    }
    &__title{
        margin: 0 0 12px 0;
        font-size: 20px;

    }
    &__description{
        font-size: 16px;
        line-height: 1.5;
    }
  }
}
</style>
