<template>
  <div
    class="w-full element1 p-[1.5px] overflow-auto rounded-t-[32px] max-w-[399px] relative"
  >
    <img
      src="/images/fourthsection/effect.png"
      class="w-full h-full absolute object-cover top-0 right-0"
      alt=""
    />
    <div class="w-full bg-black rounded-t-[32px] p-[24px] space-y-5">
      <div class="flex items-center justify-between z-10 relative">
        <div class="flex flex-col items-start">
          <span class="font-bold font-satoshi text-base text-white"
            >Jane Smith</span
          >
          <span class="text-white text-opacity-70 font-normal font-satoshi"
            >Celebrity</span
          >
        </div>
        <div class="flex items-center -space-x-4">
          <div v-for="n in 5" :key="n">
            <img src="/images/star.svg" class="w-12 h-12 object-cover" alt="" />
          </div>
        </div>
      </div>
      <p class="text-white font-medium text-lg font-satoshi z-10 relative">
        “Exceptional service! The team went above and beyond to ensure my
        privacy and safety.”
      </p>
    </div>
  </div>
</template>

<style scoped>
.border-effect {
  background: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0.25) -9.55%,
    rgba(255, 255, 255, 0) 107.38%
  );
}
</style>
