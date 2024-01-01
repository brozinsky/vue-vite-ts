<template>
  <div class="grid gap-16 items-center lg:grid-cols-2">
    <img
      :src="imageSrc"
      :alt="title"
      :class="imgClasses"
      width="568"
      height="426"
      loading="lazy"
    />
    <div class="text-center">
      <h3 class="text-xl font-semibold mb-2">{{ title }}</h3>
      <p class="text-gray-600 mb-4">{{ description }}</p>
    </div>
  </div>
</template>

<script setup lang="ts">
const props = defineProps({
  imageSrc: String,
  title: String,
  description: String,
  reversed: Boolean,
});

const imgClasses = {
  "w-full mb-4 rounded-md": true,
  "order-2": props.reversed,
};
</script>
