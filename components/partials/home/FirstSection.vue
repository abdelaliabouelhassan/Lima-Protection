<template>
  <section class="w-full relative overflow-hidden">
    <img
      src="/images/effect.png"
      class="w-full h-full absolute object-cover top-0 right-0"
      alt=""
    />

    <div
      class="w-full max-w-[1280px] grid grid-cols-1 lg:grid-cols-2 gap-14 mx-auto py-14 md:py-24 z-40 relative px-4"
    >
      <div class="w-full space-y-8">
        <div class="w-full space-y-4">
          <span
            class="font-satoshi text-white font-black text-sm text-opacity-60 uppercase"
            >{{ $t("what-we-do") }}</span
          >

          <h4 class="font-bold font-satoshi text-white text-4xl leading-[-2%]">
            {{ $t("protecting") }}
          </h4>

          <p
            class="text-white text-opacity-70 text-lg font-normal font-satoshi"
          >
            {{ $t("anticipate") }}
          </p>
        </div>
        <div class="grid grid-cols-2 gap-8">
          <div class="rounded-2xl overflow-hidden">
            <img
              src="/images/firstsection/working.png"
              class="w-full h-full object-cover"
              alt=""
            />
          </div>
          <div class="rounded-2xl overflow-hidden">
            <img
              src="/images/firstsection/serve.png"
              class="w-full h-full object-cover"
              alt=""
            />
          </div>
        </div>
      </div>

      <div class="w-full rounded-3xl overflow-hidden">
        <img
          src="/images/firstsection/bodyguard.png"
          class="w-full h-full object-cover"
          alt=""
        />
      </div>

      <div class="w-full rounded-3xl overflow-hidden">
        <img
          src="/images/firstsection/car.png"
          class="w-full h-full object-cover"
          alt=""
        />
      </div>

      <div
        class="element1 w-full h-full p-[1.5px] relative overflow-hidden rounded-[20px]"
      >
        <img
          src="/images/firstsection/effect.png"
          class="w-full h-full absolute object-cover top-0 right-0"
          alt=""
        />

        <div
          class="w-full h-full bg-black py-[32px] px-[24px] space-y-10 rounded-[20px]"
        >
          <div class="w-full flex items-start gap-4 z-40 relative">
            <div>
              <div class="w-[48px] h-[48px]">
                <img
                  src="/images/snow.svg"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
            </div>
            <div class="space-y-2">
              <h4
                class="font-satoshi font-medium text-[20px] md:text-[22px] text-white"
              >
                {{ $t("assessment") }}
              </h4>
              <p class="text-sm font-satoshi text-white text-opacity-70">
                {{ $t("conducting") }}
              </p>
            </div>
          </div>
          <div class="w-full flex items-start gap-4 z-40 relative">
            <div>
              <div class="w-[48px] h-[48px]">
                <img
                  src="/images/screen.svg"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
            </div>
            <div class="space-y-2">
              <h4
                class="font-satoshi font-medium text-[20px] md:text-[22px] text-white"
              >
                {{ $t("monitoring") }}
              </h4>
              <p class="text-sm font-satoshi text-white text-opacity-70">
                {{ $t("implementation") }}
              </p>
            </div>
          </div>
          <div class="w-full flex items-start gap-4 z-40 relative">
            <div>
              <div class="w-[48px] h-[48px]">
                <img
                  src="/images/lock.svg"
                  class="w-full h-full object-cover"
                  alt=""
                />
              </div>
            </div>
            <div class="space-y-2">
              <h4
                class="font-satoshi font-medium text-[20px] md:text-[22px] text-white"
              >
                {{ $t("comprehensive") }}
              </h4>
              <p class="text-sm font-satoshi text-white text-opacity-70">
                {{ $t("services") }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
