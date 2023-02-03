
<template>
  <header class="header">
    <div class="header-top">
      <div class="header-top-search">
        <img src="/svg/header_search_icon.svg" alt="" />
      </div>
      <a href="" class="header-logo">Candelabr</a>
      <div class="header-top-right">
        <div href="" class="header-top-right__cart">
          <a href="">
            <img src="/svg/header-shopping-cart.svg" alt="" />
          </a>
        </div>
        <div href="" class="header-top-right__profile">
          <a href="">
            <img src="/svg/header-user-avatar.svg" alt="" />
          </a>
        </div>
      </div>
    </div>
    <div class="header-menu">
        <a class="header-menu__link"
        :href="element.path"
        v-for="(element,i) of menu"
        :key="i">{{ element.name }}</a>
    </div>
  </header>
</template>

<script setup>
import { ref } from 'vue';


const menu = [
    {
        name:"Shtoto",
        path:'/plant'
    },
    {
        name:"Shtoto2",
        path:'/plant2'
    },
    {
        name:"Shtoto3",
        path:'/plant3'
    },
    {
        name:"Shtoto4",
        path:'/plant4'
    },
    {
        name:"Shtoto5",
        path:'/plant5'
    }
]
</script>




<style lang="scss" scoped>
.header {
  background: white;
  height: 132px;
  &-top {
    display: grid;
    grid-template-columns:repeat(3, 1fr) ;
    height: 70px;
    align-items: center;
    border-bottom: 1px solid rgba(0, 0, 0,.1);
    margin: 0 28px;
    &-right {
      display: flex;
      align-items: center;
      justify-content: flex-end;
      &__cart{
        margin-right: 16px;
      }
    }
  }
  &-logo {
    font-family: "Clash Display", sans-serif;
    color: #22202e;
    font-size: 24px;
    text-decoration: none;
    text-align: center;
    &:hover {
      text-decoration: underline dashed;
    }
  }
  &-menu{
    height: 62px;
    display: flex;
    justify-content: center;
    align-items: center;
    &__link{
        margin: 0 22px;
        color: #726e8d;
        text-decoration: none;
    
        &:hover{
            text-decoration: underline;
        }
    }
  }
}
</style>
