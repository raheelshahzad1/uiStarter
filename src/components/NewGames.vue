<script setup>
import Game from "./Game.vue";
import { ChevronRightIcon } from "@heroicons/vue/24/solid";
</script>
<template>
  <div class="max-w-7xl mx-auto mb-8 md:mb-20 px-4">
    
    <div class="flex justify-start items-center mb-4 gap-1">
      <h1 class="text-xl font-semibold text-gray-600">
       New Game
      </h1>
      <ChevronRightIcon class="size-4 mt-[2px] text-gray-600" />
    </div>

    <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
      <Game v-for="(item, index) in 8" :key="index" />
    </div>

  </div>
</template>