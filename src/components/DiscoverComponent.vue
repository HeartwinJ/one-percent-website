<script setup lang="ts">
import discoverBg from "@/assets/images/discover-bg.jpg";
</script>
<template>
  <div>
    <div class="text-3xl text-center">
      Discover a Range of Services to Elevate<br />Your Fitness Journey
    </div>
    <div class="relative px-32 py-8">
      <img :src="discoverBg" class="w-full" />
      <div class="absolute right-0 top-0 bottom-0 flex items-center">
        <div
          class="text-xl font-semibold bg-black p-3 flex items-center justify-center aspect-square"
        >
          Explore All
        </div>
      </div>
    </div>
  </div>
</template>
