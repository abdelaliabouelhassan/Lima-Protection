<template>
  <div class="w-full h-full">
    <HeroSection />
    <FirstSection />
    <ThirdSection />
    <FourthSection />
    <FifthSection />
    <SixthSection />
    <SeventhSection />
    <!-- <EightSection /> -->
    <NinthSection />
  </div>
</template>

<script setup>
import HeroSection from "@/components/partials/home/HeroSection.vue";
import FirstSection from "@/components/partials/home/FirstSection.vue";
import ThirdSection from "@/components/partials/home/ThirdSection.vue";
import FourthSection from "@/components/partials/home/FourthSection.vue";
import FifthSection from "@/components/partials/home/FifthSection.vue";
import SixthSection from "@/components/partials/home/SixthSection.vue";
import SeventhSection from "@/components/partials/home/SeventhSection.vue";
import EightSection from "@/components/partials/home/EightSection.vue";
import NinthSection from "@/components/partials/home/NinthSection.vue";
import { useI18n } from "vue-i18n";
const { t } = useI18n();

watchEffect(() => {
  useHead({
    link: [{ rel: "icon", type: "image/x-icon", href: "/images/favicon.png" }],
    title: t("meta-title"),
    meta: [
      { name: "description", content: t("meta-description") },
      {
        property: "og:type",
        content: "website",
      },
      {
        property: "og:title",
        content: t("meta-title"),
      },
      {
        property: "og:description",
        content: t("meta-description"),
      },
      {
        property: "og:site_name",
        content: "Lima Protection",
      },
    ],
  });
});
</script>
