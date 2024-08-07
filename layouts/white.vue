<template>
  <div class="relative w-full bg-white">
    <Header theme="light" />
    <div class="absolute top-0 left-0 w-full h-[510px]">
      <img
        src="/images/blog/mas.png"
        class="w-full h-full object-cover"
        alt=""
      />
    </div>
    <div class="relative z-30">
      <slot />
    </div>
    <Footer />
  </div>
</template>

<script setup>
import Header from "@/components/partials/Header.vue";
import Footer from "@/components/partials/Footer.vue";
</script>
