<template>
         <Product v-for="product of products"
    :key="product.id"
    :img="product.img"
    :title="product.title"
    :price="product.price"
    />
</template>



<script setup>
import { ref } from 'vue';
import Product from './Layout/Product.vue';
const products = ref([
  {
  id:1,
  img:'/img/product1.jpg',
  title:"Lorem sniper",
  price: 250,
},
{
  id:2,
  img:'/img/product2.jpg',
  title:"Lorem sniper",
  price: 150,
},
{
  id:3,
  img:'/img/product3.jpg',
  title:"Lorem sniper",
  price: 770,
},
{
  id:4,
  img:'/img/product4.jpg',
  title:"Lorem sniper",
  price: 344,
},

])
</script>