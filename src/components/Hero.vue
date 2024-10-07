<script setup>
import bg from "../assets/bg.jpg";
</script>

<template>
  <div class="w-screen h-screen">
    <!-- Background image -->
    <img
      :src="bg"
      alt="background-image"
      class="w-full h-full object-cover relative"
    />

    <!-- Hero text -->
    <h1
      class="absolute inset-0 flex items-center justify-center text-white text-7xl"
    >
      VUE BLOG
    </h1>

    <!-- Arrow icon at the bottom center -->
    <div
      class="absolute bottom-20 left-2/4 flex items-center justify-center text-white text-7xl cursor-pointer"
    >
      <!-- <TiArrowSortedDown /> -->
    </div>
  </div>
</template>

<style scoped>
/* Add any specific styles here if needed */
</style>
