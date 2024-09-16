<script setup lang="ts">
import {
  IconBrandFacebook,
  IconBrandX,
  IconBrandInstagram,
  IconBrandThreads,
  IconBrandYoutube,
} from "@tabler/icons-vue";

const quickLinks = [
  { label: "Home", url: "/" },
  { label: "Features", url: "/" },
  { label: "Testimonials", url: "/" },
  { label: "Pricing", url: "/" },
  { label: "Our Team", url: "/" },
];
const socialLinks = [
  { icon: IconBrandFacebook, url: "https://facebook.com" },
  { icon: IconBrandX, url: "https://twitter.com" },
  { icon: IconBrandInstagram, url: "https://instagram.com" },
  { icon: IconBrandThreads, url: "https://instagram.com" },
  { icon: IconBrandYoutube, url: "https://youtube.com" },
];
</script>

<template>
  <div class="bg-[#a9a9a9] text-[#0d0d0d] py-5 px-64 grid gap-16 grid-cols-3">
    <div>
      <h3 class="font-bold mb-3">About Us</h3>
      <p class="text-sm">
        BeAnkit Fit is dedicated to helping you achieve your fitness goals
        through personalized plans and expert guidance
      </p>
    </div>
    <div>
      <h3 class="font-bold mb-3">Quick Links</h3>
      <ul class="text-sm space-y-2">
        <li v-for="(link, idx) in quickLinks" :key="idx">
          <a :href="link.url">{{ link.label }}</a>
        </li>
      </ul>
    </div>
    <div>
      <h3 class="font-bold mb-3">Follow Us</h3>
      <div class="flex items-center gap-3">
        <a :href="link.url" v-for="(link, idx) in socialLinks" :key="idx">
          <component :is="link.icon" class="h-6 w-6" />
        </a>
      </div>
    </div>
  </div>
</template>
