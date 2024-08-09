<template>
  <router-link to="/blog/1" class="w-full cursor-pointer">
    <div
      class="w-full overflow-hidden bg-gray-200"
      :class="{
        ' h-[205px] sm:h-[281px] rounded-[12px] sm:rounded-2xl ':
          props.size === 'lg',
        'h-[205px] rounded-[12px]': props.size === 'sm',
      }"
    >
      <img
        :src="image"
        class="w-full h-full object-cover bg-[#F1F1F1] mix-blend-luminosity"
        alt=""
      />
    </div>
    <div class="space-y-2 pt-4">
      <span
        class="font-satoshi uppercase text-black text-sm font-black text-opacity-30"
        >{{ category }}</span
      >
      <h4
        :class="{
          ' text-2xl sm:text-[30px] sm:tracking-[-2%] sm:leading-[41.6px] ':
            props.size === 'lg',
          ' text-2xl': props.size === 'sm',
        }"
        class="text-black font-satoshi font-medium"
      >
        {{ title }}
      </h4>
      <p
        :class="{
          ' text-sm sm:text-base ': props.size === 'lg',
          ' text-sm': props.size === 'sm',
        }"
        class="font-normal text-black text-opacity-70"
        v-html="description"
      ></p>
    </div>
  </router-link>
</template>

<script setup>
const props = defineProps([
  "id",
  "title",
  "category",
  "description",
  "image",
  "size", //lg or sm
]);
</script>
