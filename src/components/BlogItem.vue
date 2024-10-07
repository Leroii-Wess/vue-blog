<script setup>
import { defineProps } from "vue";

defineProps({
  item: {
    type: Object,
    required: true,
  },
});
</script>

<template>
  <div class="p-16 bg-white">
    <!-- Title and Meta Info -->
    <div class="flex justify-center items-center flex-col">
      <h3 class="text-2xl font-medium uppercase text-blue-900">
        {{ item.title }}
      </h3>
      <p class="text-2xl font-medium uppercase text-blue-900 mt-1">
        {{ item.date }} <span class="text-orange-400">·</span>
        {{ item.comments }} COMMENTS <span class="text-orange-400">·</span> BY
        {{ item.author }}
      </p>
    </div>

    <!-- Main Content Section -->
    <div class="relative px-16">
      <p class="text-gray-700 mt-4">{{ item.text }}</p>

      <!-- Quote Section -->
      <div
        :class="{
          'mb-12 mt-20 flex flex-col gap-4 px-12 before:content-[\'\'] before:absolute before:top-[35%] before:left-16 before:h-72 before:w-px before:bg-orange-400':
            item.quote.length > 1,
          'mb-12 mt-20 flex flex-col gap-4 px-12': item.quote.length <= 1,
        }"
      >
        <p
          v-if="item.quote"
          class="text-gray-500 text-5xl uppercase leading-tight tracking-normal"
        >
          “{{ item.quote }}”
        </p>
        <p v-if="item.quoteAuthor" class="text-4xl text-gray-500 mt-2">
          — {{ item.quoteAuthor }}
        </p>
      </div>

      <!-- Button -->
      <div class="flex justify-center">
        <button
          class="px-4 py-2 text-orange-400 border border-orange-400 rounded-full hover:bg-orange-400 hover:text-white transition"
        >
          {{ item.buttonLabel }}
        </button>
      </div>

      <!-- Saved Tags -->
      <div
        class="mt-8 text-gray-500 text-2xl uppercase flex justify-center items-center"
      >
        SAVED:&nbsp;
        <span class="text-blue-900">{{ item.tags.join(", ") }}</span>
      </div>
    </div>
  </div>
</template>
