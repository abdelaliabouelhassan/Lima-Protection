<template>
  <div class="relative">
    <div class="flex items-center gap-2 cursor-pointer" @click="open = !open">
      <div>
        <img src="/images/uk.png" class="w-full h-full object-cover" alt="" />
      </div>
      <span
        class="font-satoshi uppercase"
        :class="{
          'text-white': props.theme === 'dark',
          'text-black': props.theme === 'light',
        }"
      >
        {{ locale }}</span
      >
      <div>
        <svg
          :class="{
            'text-white': props.theme === 'dark',
            'text-black': props.theme === 'light',
          }"
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="size-5"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="m19.5 8.25-7.5 7.5-7.5-7.5"
          />
        </svg>
      </div>
    </div>

    <div
      :class="{
        'bg-black text-white': props.theme === 'dark',
        ' bg-white border text-black': props.theme === 'light',
      }"
      class="absolute left-0 top-8 p-2 w-full flex flex-col gap-2 rounded-md shadow"
      v-show="open"
    >
      <button
        @click="changeLang('en')"
        class="flex items-center gap-2 cursor-pointer"
      >
        <div>
          <img src="/images/uk.png" class="w-8 h-4 object-cover" alt="" />
        </div>
        <span class="font-satoshi uppercase">en</span>
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
        <span class="font-satoshi uppercase">fr</span>
      </button>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  theme: {
    type: String,
    default: "dark",
  },
});
const open = ref(false);
import { useI18n } from "vue-i18n";
const { locale } = useI18n();

const changeLang = (lang) => {
  locale.value = lang;
  localStorage.setItem("language", lang);
  open.value = false;
};

onMounted(() => {
  if (localStorage.getItem("language")) {
    locale.value = localStorage.getItem("language");
  }
});
</script>
