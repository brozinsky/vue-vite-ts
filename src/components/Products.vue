<template>
  <section class="py-8 lg:py-16 bg-neutral-100">
    <div class="container">
        <h2 class="text-3xl font-semibold mb-4">Products</h2>
        <ul
          class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4"
        >
          <Product
            v-for="product in products"
            :key="product.id"
            :product="product"
          />
        </ul>
    </div>
  </section>
</template>

<script setup lang="ts">
import { ref } from "vue";
import Product from "./Product.vue";

const products = ref([
  { id: 1, name: "Product 1", price: 20, image:"https://picsum.photos/800/600" },
  { id: 2, name: "Product 2", price: 30, image:"https://picsum.photos/800/600" },
  { id: 3, name: "Product 3", price: 25, image:"https://picsum.photos/800/600" },
  { id: 3, name: "Product 4", price: 25, image:"https://picsum.photos/800/600" },
]);
</script>

<style scoped></style>
