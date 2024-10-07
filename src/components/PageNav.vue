<script setup>
// import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";
// import { faSearch } from "@fortawesome/free-solid-svg-icons";
</script>

<template>
  <nav
    class="fixed z-10 flex items-center justify-between bg-gray-100 opacity-80 py-2 top-0 w-full"
  >
    <div class="flex flex-shrink-0 items-center ml-20">
      <router-link class="cursor-pointer text-2xl text-gray-600" to="/">
        VUE BLOG
      </router-link>
    </div>

    <div class="m-8 flex items-center justify-center gap-4 mr-20">
      <router-link
        to="/"
        class="cursor-pointer transition ease-in-out text-blue-900 hover:text-orange-400"
      >
        HOME
      </router-link>
      <router-link
        to="/about"
        class="cursor-pointer transition ease-in-out text-blue-900 hover:text-orange-400"
      >
        ABOUT
      </router-link>
      <router-link
        to="/dropdown"
        class="cursor-pointer transition ease-in-out text-blue-900 hover:text-orange-400"
      >
        DROPDOWN
      </router-link>
      <router-link
        to="/blog"
        class="cursor-pointer transition ease-in-out text-blue-900 hover:text-orange-400"
      >
        BLOG
      </router-link>
      <router-link
        to="/contact"
        class="cursor-pointer transition ease-in-out text-blue-900 hover:text-orange-400"
      >
        CONTACT
      </router-link>
      <router-link
        to="/search"
        class="cursor-pointer hover:text-blue-700 text-orange-400"
      >
        <font-awesome-icon :icon="['fas', 'search']" />
      </router-link>
    </div>
  </nav>
</template>

<style scoped>
/* Add any component-specific styles here */
</style>
