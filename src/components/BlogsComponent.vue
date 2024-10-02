<script setup lang="ts">
import ImgYogaRoutine from "@/assets/images/blog-yoga-routine.jpg";
import ImgHiitWorkout from "@/assets/images/blog-hiit-workout.jpg";
import ImgPilatesEssentials from "@/assets/images/blog-pilates-essentials.jpg";
import ImgChestWorkout from "@/assets/images/blog-chest-workout.jpg";
import ImgMindfulMeditation from "@/assets/images/blog-mindful-meditation.jpg";

const blogs = [
  {
    title: "Morining Yoga Routine",
    img: ImgYogaRoutine,
  },
  {
    title: "HIIT Workout Guide",
    img: ImgHiitWorkout,
  },
  {
    title: "Pilates Essentials",
    img: ImgPilatesEssentials,
  },
  {
    title: "Chest Workout",
    img: ImgChestWorkout,
  },
  {
    title: "Mindful Meditation Practices",
    img: ImgMindfulMeditation,
  },
];
</script>
<template>
  <div>
    <div class="text-3xl py-4">
      <div>Blogs</div>
    </div>
    <div class="pt-4 flex items-center gap-2">
      <div
        v-for="(filter, idx) in [
          'All',
          'Basics',
          'Workout',
          'Mindset',
          'Nutrition',
          'Body Mechanism',
        ]"
        :key="idx"
        class="bg-black rounded-lg px-2 py-1"
      >
        {{ filter }}
      </div>
    </div>
    <div class="grid grid-cols-3 gap-4 pt-4">
      <div
        v-for="(item, idx) in blogs"
        :key="idx"
        class="bg-[#a9a9a9] rounded-lg flex flex-col h-full w-full"
      >
        <img :src="item.img" class="w-full" />
        <div class="p-4 flex flex-col grow">
          <div class="text-[#161616] text-xl font-bold">{{ item.title }}</div>
          <div class="py-4 grow"></div>
          <div>
            <button class="bg-black text-base rounded-lg px-2 py-1">
              Read More
            </button>
          </div>
        </div>
      </div>
      <div class="flex items-center justify-center">
        <button class="bg-black text-white px-2 py-1 rounded-lg">
          View All Posts
        </button>
      </div>
    </div>
  </div>
</template>
