<script setup lang="ts">
import HeroComponent from "@/components/HeroComponent.vue";
import RequirementsComponent from "@/components/RequirementsComponent.vue";
import DiscoverComponent from "@/components/DiscoverComponent.vue";
</script>

<template>
  <div class="space-y-5">
    <HeroComponent />
    <div class="container mx-auto sm:px-6 lg:px-8 space-y-5">
      <RequirementsComponent />
      <DiscoverComponent />
    </div>
  </div>
</template>
