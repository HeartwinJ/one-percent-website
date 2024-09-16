<script setup lang="ts">
import { RouterLink } from "vue-router";
import { IconLaurelWreath1, IconShoppingCart } from "@tabler/icons-vue";

const navLinks = [
  { label: "Home", path: "/" },
  { label: "Blog", path: "/blog" },
  { label: "Testimonials", path: "/testimonials" },
  { label: "Pricing", path: "/pricing" },
  { label: "About", path: "/about" },
  { label: "Contact", path: "/contact" },
  { label: "Course", path: "/course" },
];
</script>
<template>
  <header class="flex justify-between items-center p-5">
    <IconLaurelWreath1 class="h-10 w-10" />
    <nav>
      <ul class="flex space-x-5">
        <li v-for="(link, idx) in navLinks" :key="idx">
          <RouterLink :to="link.path" active-class="border-b-2">{{
            link.label
          }}</RouterLink>
        </li>
      </ul>
    </nav>
    <button
      class="flex items-center gap-4 text-black bg-white rounded-lg px-4 py-2"
    >
      <IconShoppingCart class="h-6 w-6" />
      <span class="font-semibold tracking-wider">Cart</span>
    </button>
  </header>
</template>
