<template>
  <header class="w-full absolute top-0 left-0 z-50">
    <div
      class="w-full max-w-[1313px] mx-auto flex items-center justify-between px-4 pb-4 pt-8 z-50 relative"
    >
      <router-link to="/">
        <img
          src="/images/logo.svg"
          class="w-full h-full object-cover"
          alt=""
          v-if="props.theme === 'dark'"
        />
        <img
          src="/images/logo-dark.svg"
          class="w-full h-full object-cover"
          alt=""
          v-else
        />
      </router-link>

      <div class="element rounded-full p-px hidden lg:block">
        <div
          :class="{
            'bg-[#00000003] border text-[#0000004D] border-[#0000000D]':
              props.theme === 'light',
            'bg-black text-white text-opacity-50': props.theme === 'dark',
          }"
          class="rounded-full py-[12px] px-[32px] flex items-center justify-between gap-9"
        >
          <router-link
            to="/about-us"
            :class="{
              ' text-black': pageName === 'about-us' && props.theme === 'light',
              '  text-[#0000004D] ':
                pageName != 'about-us' && props.theme === 'light',
              'bg-black text-white text-opacity-50 ': props.theme === 'dark',
            }"
            class="font-satoshi text-base font-normal hover:text-opacity-100 duration-200"
          >
            About us
          </router-link>
          <router-link
            to="/blog"
            :class="{
              ' text-black': pageName === 'blog' && props.theme === 'light',
              '  text-[#0000004D] ':
                pageName != 'blog' && props.theme === 'light',
              'bg-black text-white text-opacity-50 ': props.theme === 'dark',
            }"
            class="font-satoshi text-base font-normal hover:text-opacity-100 duration-200"
          >
            Blog
          </router-link>
          <router-link
            to="/customers"
            :class="{
              ' text-black':
                pageName === 'customers' && props.theme === 'light',
              '  text-[#0000004D] ':
                pageName != 'customers' && props.theme === 'light',
              'bg-black text-white text-opacity-50 ': props.theme === 'dark',
            }"
            class="font-satoshi text-base font-normal hover:text-opacity-100 duration-200"
          >
            Customers
          </router-link>
          <router-link
            to="/resources"
            :class="{
              ' text-black':
                pageName === 'resources' && props.theme === 'light',
              '  text-[#0000004D] ':
                pageName != 'resources' && props.theme === 'light',
              'bg-black text-white text-opacity-50 ': props.theme === 'dark',
            }"
            class="font-satoshi text-base font-normal hover:text-opacity-100 duration-200"
          >
            Resources
          </router-link>

          <div
            :class="{
              '  bg-black bg-opacity-5 ': props.theme === 'light',
              'bg-white bg-opacity-20 ': props.theme === 'dark',
            }"
            class="h-[26px] w-px"
          ></div>

          <LanguageSwitch :theme="props.theme" />
        </div>
      </div>

      <div class="items-center gap-4 hidden lg:flex">
        <a
          href="#"
          :class="{
            '  text-black ': props.theme === 'light',
            'text-white text-opacity-60 ': props.theme === 'dark',
          }"
          class="font-satoshi hover:text-opacity-100 duration-200"
          >Apply</a
        >
        <a
          href="https://ax6hl0zetxi.typeform.com/to/ehMKwuTo"
          target="_blank"
          :class="{
            '  bg-black text-white ': props.theme === 'light',
            'bg-white  text-black hover:shadow-[0px_0px_25px_rgba(255,255,255,0.5)]':
              props.theme === 'dark',
          }"
          class="hover:shadow-lg whitespace-nowrap font-satoshi font-medium py-[12px] px-[24px] rounded-full duration-200"
        >
          {{ $t("hire-us") }}
        </a>
      </div>

      <button
        name="menu1"
        @click="showMenu = !showMenu"
        :class="{
          '  text-black ': props.theme === 'light',
          'text-white text-opacity-70 ': props.theme === 'dark',
        }"
        class="h-fit lg:hidden"
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
          <router-link
            to="/about-us"
            class="font-satoshi text-white text-2xl text-opacity-50 font-normal hover:text-opacity-100 duration-200"
          >
            About us
          </router-link>
          <router-link
            to="/blog"
            class="font-satoshi text-white text-2xl text-opacity-50 font-normal hover:text-opacity-100 duration-200"
          >
            Blog
          </router-link>
          <router-link
            to="/customers"
            class="font-satoshi text-white text-2xl text-opacity-50 font-normal hover:text-opacity-100 duration-200"
          >
            Customers
          </router-link>
          <router-link
            to="/resources"
            class="font-satoshi text-white text-2xl text-opacity-50 font-normal hover:text-opacity-100 duration-200"
          >
            Resources
          </router-link>
          <LanguageSwitch />

          <div class="flex items-center flex-col gap-4">
            <a
              href="#"
              class="text-white text-opacity-60 font-satoshi hover:text-opacity-100 duration-200"
              >Apply</a
            >
            <a
              href="https://ax6hl0zetxi.typeform.com/to/ehMKwuTo"
              target="_blank"
              class="text-black font-satoshi hover:shadow-[0px_0px_25px_rgba(255,255,255,0.5)] font-medium bg-white py-[12px] px-[24px] rounded-full duration-200"
            >
              {{ $t("hire-us") }}
            </a>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script setup>
import LanguageSwitch from "@/components/UI/LanguageSwitch.vue";

const props = defineProps({
  theme: {
    type: String,
    default: "dark",
  },
});

const open = ref(false);
const showMenu = ref(false);
const route = useRoute();
const pageName = computed(() => route.name);

watch(showMenu, (newValue, oldValue) => {
  document.body.classList.toggle("overflow-hidden");
});
</script>
