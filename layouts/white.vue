<template>
  <div class="relative w-full bg-white">
    <Header theme="light" />
    <slot />
    <Footer />
  </div>
</template>

<script setup>
import Header from "@/components/partials/Header.vue";
import Footer from "@/components/partials/Footer.vue";
</script>
