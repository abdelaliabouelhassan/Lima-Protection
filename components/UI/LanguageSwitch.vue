<template>
  <div class="relative">
    <div class="flex items-center gap-2 cursor-pointer" @click="open = !open">
      <div>
        <img src="/images/uk.png" class="w-full h-full object-cover" alt="" />
      </div>
      <span class="font-satoshi text-white">EN</span>
      <div>
        <svg
          width="12"
          height="6"
          viewBox="0 0 12 6"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M10.5 0.75L6 5.25L1.5 0.749999"
            stroke="white"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>
      </div>
    </div>

    <div
      class="absolute left-0 top-8 p-2 bg-black w-full flex flex-col gap-2 rounded"
      v-show="open"
    >
      <div
        class="flex items-center gap-2 cursor-pointer"
        v-for="n in 2"
        :key="n"
      >
        <div>
          <img src="/images/uk.png" class="w-full h-full object-cover" alt="" />
        </div>
        <span class="font-satoshi text-white">FR</span>
      </div>
    </div>
  </div>
</template>

<script setup>
const open = ref(false);
</script>
