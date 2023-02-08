<template>
  <div class="products-container">
    <div class="products">
      <Product
        v-for="product of products"
        :key="product.id"
        :img="product.img"
        :title="product.title"
        :price="product.price"
      />
    </div>
    <a href="" class="products-link">View collection</a>
  </div>
</template>

<script setup>
import { ref } from "vue";
import Product from "./Layout/Product.vue";
const products = ref([
  {
    id: 1,
    img: "/img/product1.jpg",
    title: "Lorem sniper",
    price: 250,
  },
  {
    id: 2,
    img: "/img/product2.jpg",
    title: "Lorem sniper",
    price: 150,
  },
  {
    id: 3,
    img: "/img/product3.jpg",
    title: "Lorem sniper",
    price: 770,
  },
  {
    id: 4,
    img: "/img/product4.jpg",
    title: "Lorem sniper",
    price: 344,
  },
]);
</script>

<style lang="scss" scoped>
@import url("https://fonts.cdnfonts.com/css/clash-display");
.products {
  padding: 0 80px;
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  column-gap: 20px;
  margin-bottom: 64px;
  &-container {
    margin-bottom: 56px;
  }
  &-link {
    display: block;
    text-align: center;
    color: #2a254b;
    font-family: 'Clash Display', sans-serif;
    text-decoration: none;
    &:hover{
        text-decoration: underline;
    }
  }
}
</style>
