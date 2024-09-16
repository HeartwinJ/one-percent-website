<script setup lang="ts">
import heroBg from "@/assets/images/hero-bg.jpg";
</script>
<template>
  <div class="relative">
    <img :src="heroBg" class="w-full" />
    <div class="absolute bottom-0 left-0 p-3 w-1/3 space-y-3">
      <div class="text-6xl space-y-3">
        <div>Achieve Your</div>
        <div class="uppercase">dream physique</div>
      </div>
      <div class="text-xl">
        Welcome to BeAnkit Fit, where we specialize in transforming lives
        through personalized fitness programs. Our team of certified trainers is
        dedicated to helping you reach your fitness goals with tailored workouts
        and expert guidance.
      </div>
      <div class="flex items-center justify-center w-full gap-3">
        <button class="px-5 py-2 text-sm bg-black text-white rounded-lg">
          Join Now
        </button>
        <button class="px-5 py-2 text-sm bg-white text-black rounded-lg">
          Learn More
        </button>
      </div>
    </div>
  </div>
</template>
