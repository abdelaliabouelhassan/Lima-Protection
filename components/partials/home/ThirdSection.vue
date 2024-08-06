<template>
  <section class="w-full py-20 space-y-14">
    <div class="flex flex-col items-center gap-6 px-4 text-center">
      <span
        class="font-satoshi font-black text-sm text-white text-opacity-60 uppercase"
        >our experiences</span
      >

      <h3 class="text-white font-satoshi font-bold text-4xl">
        Diverse expertise for diverse customers
      </h3>

      <a
        href="https://ax6hl0zetxi.typeform.com/to/ehMKwuTo"
        target="_blank"
        class="text-black font-satoshi font-medium text-base bg-white py-[12px] px-[24px] rounded-full hover:shadow-[0px_0px_25px_rgba(255,255,255,0.5)] duration-200"
      >
        {{ $t("hire-us") }}
      </a>
    </div>

    <div
      class="grid grid-cols-1 xl:grid-cols-2 gap-6 max-w-[1280px] mx-auto xl:px-0 px-4"
    >
      <ClientsCard />
      <div class="w-full flex flex-col gap-6">
        <ServicesCard />
        <PortfolioCard />
      </div>
    </div>
  </section>
</template>

<script setup>
import ClientsCard from "@/components/UI/ClientsCard.vue";
import ServicesCard from "@/components/UI/ServicesCard.vue";
import PortfolioCard from "@/components/UI/PortfolioCard.vue";
</script>
