<script setup>
// Import necessary components and assets
import BlogItem from "./BlogItem.vue";
// import Slider from './Slider.vue';
import { blogInfo } from "../constants/data";
import camper from "../assets/Camper-1.jpg";
import flowerShop from "../assets/Flower-Shop.jpg";
</script>

<template>
  <div class="bg-gray-100 py-44 flex justify-center">
    <div class="w-[60%] mx-auto">
      <!-- First Section: Slider and First Blog Item -->
      <!-- <div class="mb-12">
        <Slider />
        <BlogItem :item="blogInfo[0]" />
      </div> -->

      <!-- Second Section: Image and Second Blog Item -->
      <div class="mb-12">
        <img :src="camper" alt="camping-bus" />
        <BlogItem :item="blogInfo[1]" />
      </div>

      <!-- Third Section: Image and Third Blog Item -->
      <div>
        <img :src="flowerShop" alt="flower-shop" />
        <BlogItem :item="blogInfo[2]" />
      </div>
    </div>
  </div>
</template>
