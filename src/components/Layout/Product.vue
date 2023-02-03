<template>
    <div class="product">
        <a>
            <img class="product-image"
            :src="img" :alt="title">
        </a>
        <a class="product-name">{{ title }}</a>
        <span class="product-price">{{ price }}грн</span>
    </div>
</template>


<script setup>
const props = defineProps ({
   img:{
    type: String,
    required: true,
   },
   title:{
    type: String,
    required: true,
   },
   price:{
    type: Number,
    required: true,
   },
})

</script>