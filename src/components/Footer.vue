<script setup>
import profilePhoto from "../assets/about-me.jpg";
import gallery from "../assets/gallery.png";
</script>

<template>
  <div class="bg-white-100 py-32 justify-center">
    <div class="flex flex-wrap gap-20 place-content-around mx-32">
      <!-- Profile Section -->
      <div class="flex flex-col gap-8 w-1/5">
        <div class="flex items-center justify-center rounded-full">
          <img
            :src="profilePhoto"
            alt="profile-photo"
            class="h-28 w-28 rounded-full"
          />
        </div>

        <div class="flex flex-col justify-center items-center gap-6">
          <h3 class="font-bold text-2xl uppercase text-gray-600">- Claire -</h3>
          <p class="text-gray-600">
            Hi, my name is Clare and I'm a serial blogger. I love life and more
            than anything in the whole wide world, I love taking photographs. Oh
            and did I mention, I quite like blogging?
          </p>
        </div>
      </div>

      <!-- Recent Posts Section -->
      <div class="flex flex-col gap-4 w-1/5 items-center">
        <h3 class="font-bold text-2xl text-gray-600 uppercase">
          - Recent Posts -
        </h3>
        <ul class="flex flex-col gap-6 items-center">
          <li>
            <a
              class="text-gray-600 hover:text-orange-300 transition-all"
              href="#"
            >
              The Lollipop
            </a>
          </li>
          <li>
            <a
              class="text-gray-600 hover:text-orange-300 transition-all"
              href="#"
            >
              Running Through Nigeria
            </a>
          </li>
          <li>
            <a
              class="text-gray-600 hover:text-orange-300 transition-all"
              href="#"
            >
              The Apothecary
            </a>
          </li>
          <li>
            <a
              class="text-gray-600 hover:text-orange-300 transition-all"
              href="#"
            >
              The Flowers
            </a>
          </li>
          <li>
            <a
              class="text-gray-600 hover:text-orange-300 transition-all"
              href="#"
            >
              The Sunny Day
            </a>
          </li>
        </ul>
      </div>

      <!-- Categories Section -->
      <div class="flex flex-col gap-4 w-1/5 items-center">
        <h3 class="font-bold text-2xl text-gray-600 uppercase">
          - Categories -
        </h3>
        <ul class="flex flex-col gap-6 items-center">
          <li>
            <a
              class="text-gray-600 hover:text-orange-300 transition-all"
              href="#"
            >
              Cute
            </a>
          </li>
          <li>
            <a
              class="text-gray-600 hover:text-orange-300 transition-all"
              href="#"
            >
              Fun
            </a>
          </li>
          <li>
            <a
              class="text-gray-600 hover:text-orange-300 transition-all"
              href="#"
            >
              Fitness
            </a>
          </li>
          <li>
            <a
              class="text-gray-600 hover:text-orange-300 transition-all"
              href="#"
            >
              Healthy
            </a>
          </li>
        </ul>
      </div>

      <!-- Gallery Section -->
      <div class="flex flex-col gap-4 w-1/5 items-center">
        <h3 class="font-bold text-2xl text-gray-600 uppercase">- Gallery -</h3>
        <div>
          <img :src="gallery" alt="gallery" />
        </div>
      </div>
    </div>
  </div>
</template>
