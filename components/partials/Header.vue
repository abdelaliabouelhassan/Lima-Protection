<template>
  <header class="w-full absolute top-0 left-0 z-50">
    <div
      class="w-full max-w-[1313px] mx-auto flex items-center justify-between px-4 pb-4 pt-8"
    >
      <div>
        <img src="/images/logo.svg" class="w-full h-full object-cover" alt="" />
      </div>

      <div class="element rounded-full p-px hidden lg:block">
        <div
          class="bg-black rounded-full py-[12px] px-[32px] flex items-center justify-between gap-9"
        >
          <a
            href="#"
            class="font-satoshi text-white text-opacity-50 text-base font-normal hover:text-opacity-100 duration-200"
          >
            About us
          </a>
          <a
            href="#"
            class="font-satoshi text-white text-opacity-50 text-base font-normal hover:text-opacity-100 duration-200"
          >
            Blog
          </a>
          <a
            href="#"
            class="font-satoshi text-white text-opacity-50 text-base font-normal hover:text-opacity-100 duration-200"
          >
            Customers
          </a>
          <a
            href="#"
            class="font-satoshi text-white text-opacity-50 text-base font-normal hover:text-opacity-100 duration-200"
          >
            Resources
          </a>

          <div class="h-[26px] w-px bg-white bg-opacity-20"></div>

          <LanguageSwitch />
        </div>
      </div>

      <div class="items-center gap-4 hidden lg:flex">
        <a
          href="#"
          class="text-white text-opacity-60 font-satoshi hover:text-opacity-100 duration-200"
          >Apply</a
        >
        <button
          class="text-black hover:shadow-[0px_0px_25px_rgba(255,255,255,0.5)] font-satoshi font-medium bg-white py-[12px] px-[24px] rounded-full duration-200"
        >
          Hire us
        </button>
      </div>

      <button
        name="menu1"
        @click="showMenu = !showMenu"
        class="h-fit lg:hidden text-white text-opacity-70"
      >
        <svg
          width="43"
          height="29"
          viewBox="0 0 43 29"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M2.5 2.5H40.5"
            stroke="currentColor"
            stroke-width="5"
            stroke-linecap="round"
          />
          <path
            d="M2.5 14.5H40.5"
            stroke="currentColor"
            stroke-width="5"
            stroke-linecap="round"
          />
          <path
            d="M2.5 26.5H40.5"
            stroke="currentColor"
            stroke-width="5"
            stroke-linecap="round"
          />
        </svg>
      </button>
    </div>

    <div
      class="lg:hidden overflow-hidden absolute top-0 z-50 bg-black bg-gradient-to-b from-[#ffffff30] from-[9.11%] to-[#00000001] to-[76.61%] h-screen w-full flex flex-col transition-all duration-500 ease-in-out overflow-y-auto"
      :class="{ '-translate-y-full': !showMenu }"
    >
      <div class="z-40 flex justify-between py-4 px-8 w-full">
        <router-link
          @click="showMenu = !showMenu"
          to="/"
          class="h-full"
          aria-label="svglogo"
        >
          <img src="/images/logo.svg" alt="" srcset="" />
        </router-link>
        <button
          name="menu2"
          class="h-fit lg:hidden text-white text-opacity-70 pt-1"
          @click="showMenu = !showMenu"
        >
          <svg
            width="43"
            height="33"
            viewBox="0 0 43 33"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M3 3L29.8701 29.8701"
              stroke="white"
              stroke-width="5"
              stroke-linecap="round"
            />
            <path
              d="M3 30L29.8701 3.12994"
              stroke="white"
              stroke-width="5"
              stroke-linecap="round"
            />
          </svg>
        </button>
      </div>
      <!-- small screen menu links-->
      <div
        class="lg:hidden h-full overflow-hidden flex justify-center items-center text-white font-satoshi font-bold"
      >
        <div
          class="w-full h-full justify-center flex flex-col items-center space-y-8 px-4 pb-8 overflow-y-auto"
        >
          <a
            href="#"
            class="font-satoshi text-white text-2xl text-opacity-50 font-normal hover:text-opacity-100 duration-200"
          >
            About us
          </a>
          <a
            href="#"
            class="font-satoshi text-white text-2xl text-opacity-50 font-normal hover:text-opacity-100 duration-200"
          >
            Blog
          </a>
          <a
            href="#"
            class="font-satoshi text-white text-2xl text-opacity-50 font-normal hover:text-opacity-100 duration-200"
          >
            Customers
          </a>
          <a
            href="#"
            class="font-satoshi text-white text-2xl text-opacity-50 font-normal hover:text-opacity-100 duration-200"
          >
            Resources
          </a>
          <LanguageSwitch />

          <div class="flex items-center flex-col gap-4">
            <a
              href="#"
              class="text-white text-opacity-60 font-satoshi hover:text-opacity-100 duration-200"
              >Apply</a
            >
            <button
              class="text-black font-satoshi hover:shadow-[0px_0px_25px_rgba(255,255,255,0.5)] font-medium bg-white py-[12px] px-[24px] rounded-full duration-200"
            >
              Hire us
            </button>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script setup>
import LanguageSwitch from "@/components/UI/LanguageSwitch.vue";
const open = ref(false);
const showMenu = ref(false);

watch(showMenu, (newValue, oldValue) => {
  document.body.classList.toggle("overflow-hidden");
});
</script>
