<template>
  <section class="w-full pt-20 pb-40 space-y-14">
    <div class="flex flex-col items-center gap-6 px-4 text-center">
      <span
        class="font-satoshi font-black text-sm text-white text-opacity-60 uppercase"
        >{{ $t("process") }}</span
      >

      <h3 class="text-white font-satoshi font-bold text-4xl">
        {{ $t("confident") }}
      </h3>

      <button
        class="text-black font-satoshi font-medium text-base bg-white py-[12px] px-[24px] rounded-full hover:shadow-[0px_0px_25px_rgba(255,255,255,0.5)] duration-200"
      >
        {{ $t("get-started") }}
      </button>
    </div>

    <div
      class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8 max-w-[1280px] mx-auto px-4 xl:px-0"
    >
      <div class="w-full flex flex-col items-center -space-y-28">
        <div>
          <img
            src="/images/sixthsection/Targeted.svg"
            class="w-full h-full object-cover"
            alt=""
          />
        </div>

        <div class="w-full text-center space-y-4">
          <h3 class="text-white font-medium font-satoshi text-xl">
            {{ $t("targeted") }}
          </h3>
          <p
            class="text-sm text-white text-opacity-70 font-satoshi font-normal"
          >
            {{ $t("recruitment") }}
          </p>
        </div>
      </div>
      <div class="w-full flex flex-col items-center -space-y-28">
        <div>
          <img
            src="/images/sixthsection/Specialized.svg"
            class="w-full h-full object-cover"
            alt=""
          />
        </div>

        <div class="w-full text-center space-y-4">
          <h3 class="text-white font-medium font-satoshi text-xl">
            {{ $t("specialized") }}
          </h3>
          <p
            class="text-sm text-white text-opacity-70 font-satoshi font-normal"
          >
            {{ $t("search") }}
          </p>
        </div>
      </div>
      <div class="w-full flex flex-col items-center -space-y-28">
        <div>
          <img
            src="/images/sixthsection/Rigorous.svg"
            class="w-full h-full object-cover"
            alt=""
          />
        </div>

        <div class="w-full text-center space-y-4">
          <h3 class="text-white font-medium font-satoshi text-xl">
            {{ $t("rigorous") }}
          </h3>
          <p
            class="text-sm text-white text-opacity-70 font-satoshi font-normal"
          >
            {{ $t("careful") }}
          </p>
        </div>
      </div>
    </div>
  </section>
</template>
