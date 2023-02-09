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
    <div class="products-link">
      <uiButton color="lightgray" type="link" to="/">Lorem, ipsum.</uiButton>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
import Product from "@/components/Layout/Product.vue";
import uiButton from "@/components/UI/Button.vue";
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
    text-align: center;
  }
}
</style>
