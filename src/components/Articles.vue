<script setup>
import { onMounted } from "vue";
import { articles } from "../constants/data";
import ArticleCard from "./ArticleCard.vue";
</script>

<template>
  <div class="bg-white py-32 flex flex-col gap-4 justify-center">
    <!-- Section title -->
    <div class="flex justify-center items-center">
      <h2 class="flex text-center pb-8">- OUR ARTICLES -</h2>
    </div>

    <!-- Article cards -->
    <div class="flex flex-wrap gap-4 justify-center">
      <ArticleCard v-for="card in articles" :key="card.title" :card="card" />
    </div>
  </div>
</template>
