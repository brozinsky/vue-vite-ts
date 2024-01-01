<template>
  <footer class="bg-gray-800 text-white py-4 text-center">
    <p>&copy; {{ currentYear }} Company. All rights reserved.</p>
  </footer>
</template>

<script setup lang="ts">
const currentYear = new Date().getFullYear();
</script>
