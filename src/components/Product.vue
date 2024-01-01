<template>
    <div class="max-w-sm bg-white border border-gray-200 rounded-lg shadow">
      <img :src="product.image" alt="Product Image" class="rounded-t-lg" width="311" height="233" loading="lazy"/>
      <div class="p-5">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900">{{ product.name }}</h5>
        <p class="mb-2 text-lg font-semibold text-gray-700">${{ product.price.toFixed(2) }}</p>
        <p class="mb-3 font-normal text-gray-700">{{ product.description }}</p>
        <Button withIcon>
          Read more
        </Button>
      </div>
    </div>
  </template>
  
  <script setup lang="ts">
  import { PropType } from 'vue';
  import Button from './Button.vue';
  const props = defineProps({
    product: {
      type: Object as PropType<{ id: number; name: string; price: number }>,
      required: true,
    },
  });
  </script>
  
  <style scoped>
  /* Additional styling for individual products */
  li {
    transition: transform 0.2s ease-in-out;
  }
  
  li:hover {
    transform: scale(1.05);
  }
  </style>