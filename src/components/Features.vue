<template>
  <section class="py-8 lg:py-16">
    <div class="container">
      <div class="space-y-16">
        <Feature
          imageSrc="https://picsum.photos/500/350"
          title="Feature 1"
          description="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque euismod, nisl sed tincidunt efficitur, justo leo cursus turpis."
        />
        <Feature
          imageSrc="https://picsum.photos/500/350"
          title="Feature 2"
          description="Sed eget justo vel tellus vulputate semper. Morbi malesuada, orci ut convallis dapibus, leo justo fermentum libero."
          reversed
        />
        <Feature
          imageSrc="https://picsum.photos/500/350"
          title="Feature 3"
          description="Fusce ultricies justo eget justo fringilla euismod. Sed vitae justo non mauris gravida sagittis vel eu elit."
        />
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
import Feature from "./Feature.vue";
</script>
