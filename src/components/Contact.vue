<template>
  <section class="py-8 lg:py-16">
    <div class="container">
      <h2 class="text-3xl font-semibold mb-4">Contact</h2>
      <p class="text-gray-600 mb-4">Feel free to reach out to us via email:</p>
      <Button @click="sendEmail" withIcon> Mail to Contact </Button>
    </div>
  </section>
</template>

<script setup lang="ts">
import Button from "./Button.vue";

const sendEmail = () => {
  window.location.href = "mailto:contact@example.com";
};
</script>

<style scoped></style>
