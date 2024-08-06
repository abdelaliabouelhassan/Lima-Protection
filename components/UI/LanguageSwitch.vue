<template>
  <div class="relative">
    <div class="flex items-center gap-2 cursor-pointer" @click="open = !open">
      <div>
        <img src="/images/uk.png" class="w-full h-full object-cover" alt="" />
      </div>
      <span class="font-satoshi text-white uppercase">
        {{ locale }} - {{ $t("hello") }}</span
      >
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
      <button
        @click="changeLang('en')"
        class="flex items-center gap-2 cursor-pointer"
      >
        <div>
          <img src="/images/uk.png" class="w-8 h-4 object-cover" alt="" />
        </div>
        <span class="font-satoshi text-white uppercase">en</span>
      </button>
      <button
        @click="changeLang('fr')"
        class="flex items-center gap-2 cursor-pointer"
      >
        <div>
          <img
            src="https://upload.wikimedia.org/wikipedia/en/c/c3/Flag_of_France.svg"
            class="w-8 h-4 object-cover"
            alt=""
          />
        </div>
        <span class="font-satoshi text-white uppercase">fr</span>
      </button>
    </div>
  </div>
</template>

<script setup>
const open = ref(false);
import { useI18n } from "vue-i18n";
const { locale } = useI18n();

const changeLang = (lang) => {
  locale.value = lang;
  localStorage.setItem("language", lang);
};

onMounted(() => {
  if (localStorage.getItem("language")) {
    locale.value = localStorage.getItem("language");
  }
});
</script>
