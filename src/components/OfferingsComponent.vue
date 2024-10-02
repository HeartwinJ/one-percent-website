<script setup lang="ts"></script>
<template>
  <div>
    <div class="text-3xl flex items-center justify-between py-4">
      <div>Explore Our Offerings</div>
      <button class="text-base bg-black rounded-lg p-2">View All</button>
    </div>
    <div class="grid grid-cols-2 gap-8 pt-4">
      <div
        v-for="(offering, idx) in [
          'Strength',
          'Cardio',
          'Yoga',
          'Nutrition',
          'Personalized',
          'Mindfulness',
        ]"
        :key="idx"
        class="flex items-center gap-6 text-2xl"
      >
        <div>{{ idx + 1 }}</div>
        <div class="grow h-0.5 bg-white/30 rounded-full"></div>
        <div>{{ offering }}</div>
      </div>
    </div>
  </div>
</template>
