<template>
  <div class="w-full h-full">
    <FirstSection />
    <SecondSection />
  </div>
</template>

<script setup>
import FirstSection from "@/components/partials/blog/FirstSection.vue";
import SecondSection from "@/components/partials/blog/SecondSection.vue";
definePageMeta({
  layout: "white",
});
</script>
