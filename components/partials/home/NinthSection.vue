<template>
  <section class="w-full -space-y-60">
    <div class="w-full relative overflow-hidden h-[35rem]">
      <div class="absolute w-full top-28">
        <div class="flex flex-col items-center gap-6 px-4 text-center pt-4">
          <span
            class="font-satoshi font-black text-sm text-white text-opacity-60 uppercase"
            >{{ $t("lets") }}</span
          >

          <h3 class="text-white font-satoshi font-bold text-4xl">
            {{ $t("ready") }}
          </h3>

          <a
            href="https://ax6hl0zetxi.typeform.com/to/ehMKwuTo"
            target="_blank"
            class="element rounded-full p-px group duration-300"
          >
            <div
              class="rounded-full py-[12px] px-[20px] text-white font-satoshi font-medium bg-black duration-300 bg-gradient-to-br group-hover:from-[#ffffff80] group-hover:to-[#00000001] from-[#ffffff30] from-[9.11%] to-[#00000001] to-[76.61%]"
            >
              {{ $t("hire-us") }}
            </div>
          </a>
        </div>
      </div>

      <img
        src="/images/rounded-effect.png"
        class="w-full h-full object-cover mt-[14rem]"
        alt=""
      />
    </div>
  </section>
</template>
