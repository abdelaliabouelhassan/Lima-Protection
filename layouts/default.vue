<template>
  <div class="relative w-full bg-black">
    <Header class="absolute top-0 left-0 z-50" />
    <slot />
  </div>
</template>

<script setup>
import Header from "@/components/partials/Header.vue";
</script>
