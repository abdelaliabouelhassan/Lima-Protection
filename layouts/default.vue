<template>
  <div class="relative w-full bg-black">
    <Header />
    <slot />
  </div>
</template>

<script setup>
import Header from "@/components/partials/Header.vue";
</script>
