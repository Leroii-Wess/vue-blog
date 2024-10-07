<script setup>
import { defineProps } from "vue";

defineProps({
  card: {
    type: String,
  },
});
</script>

<template>
  <div class="px-10 w-[480px]">
    <!-- Blog Image -->
    <div class="w-full">
      <img
        :src="card.image"
        alt="blog-image"
        class="w-full h-full object-cover hover:scale-105 overflow-hidden transition-all hover:grayscale-[30%]"
      />
    </div>

    <!-- Article Content -->
    <div
      class="px-6 py-16 h-1/5 p-4 flex flex-col gap-2 content-center justify-center text-center"
    >
      <span
        class="uppercase font-semibold hover:text-orange-400 transition-all text-gray-800"
      >
        <router-link :to="'/'">{{ card.title }}</router-link>
      </span>
      <span class="text-gray-600">{{ card.date }}</span>
    </div>
  </div>
</template>
