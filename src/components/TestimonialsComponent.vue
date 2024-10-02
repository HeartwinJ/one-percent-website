<script setup lang="ts">
const testimonials = [
  {
    name: "Heartwin",
    img: "https://randomuser.me/api/portraits/men/11.jpg",
    service: "Muscle gain and fat loss",
    testimony:
      "BeAnkit Fit has transformed my fitness journey. Highly recommended!",
  },
  {
    name: "Krishna",
    img: "https://randomuser.me/api/portraits/men/6.jpg",
    service: "Muscle gain",
    testimony:
      "Training with BeAnkit Fit has improved my flexibility and strength.",
  },
  {
    name: "Sudeep",
    img: "https://randomuser.me/api/portraits/men/12.jpg",
    service: "Fat loss",
    testimony: "The personalized training plans have boosted my performance.",
  },
];
</script>
<template>
  <div>
    <div class="text-3xl py-4">
      <div>Client Testimonials</div>
    </div>
    <div class="p-8 bg-[#a9a9a9] rounded-lg">
      <div class="grid grid-cols-3 gap-4">
        <div
          v-for="(testimonial, idx) in testimonials"
          :key="idx"
          class="text-black"
        >
          <div class="flex gap-2 items-center">
            <img :src="testimonial.img" class="w-16 h-16 rounded-full" />
            <div class="flex flex-col">
              <div class="text-lg font-bold">{{ testimonial.name }}</div>
              <div class="text-sm">{{ testimonial.service }}</div>
            </div>
          </div>
          <div class="pt-4 text-sm">"{{ testimonial.testimony }}""</div>
        </div>
      </div>
      <div class="flex items-center justify-center pt-8">
        <button class="bg-black text-white px-4 py-1 rounded-lg">
          Explore
        </button>
      </div>
    </div>
  </div>
</template>
