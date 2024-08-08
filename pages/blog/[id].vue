<template>
  <div class="w-full h-full">
    <FirstSection />
    <SecondSection />
    <ThirdSection />
  </div>
</template>

<script setup>
import FirstSection from "@/components/partials/blog-details/FirstSection.vue";
import SecondSection from "@/components/partials/blog-details/SecondSection.vue";
import ThirdSection from "@/components/partials/blog-details/ThirdSection.vue";
definePageMeta({
  layout: "white",
});
</script>
