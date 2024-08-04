<template>
  <div
    class="element1 p-[1.5px] rounded-[20px] w-full relative overflow-hidden"
  >
    <img
      src="/images/firstsection/effect.png"
      class="w-full h-full absolute object-cover top-0 right-0"
      alt=""
    />
    <div class="w-full py-[32px] bg-black rounded-[20px] space-y-10">
      <div class="w-full space-y-2 px-[24px] relative z-10">
        <h3 class="text-white font-satoshi font-bold text-2xl">
          Large portfolio
        </h3>
        <p class="text-base font-satoshi text-white text-opacity-70">
          Established reputation with a diverse client portfolio demonstrating
          our ability to meet the varied requirements of our clients.
        </p>
      </div>
      <div class="w-full relative space-y-4">
        <Splide
          @splide:mounted="splideMounted"
          :extensions="extensions"
          :options="options"
          @mouseover="startScroll"
          @mouseleave="stopScroll"
        >
          <SplideSlide v-for="(item, index, key) in Portfolio" :key="key">
            <div
              class="rounded-full bg-card flex py-[12px] px-[20px] font-satoshi font-medium border border-[#FFFFFF1A] bg-black duration-300"
            >
              <span
                class="gradient-text whitespace-nowrap text-center text-sm m-auto"
                >{{ item.title }}</span
              >
            </div>
          </SplideSlide>
        </Splide>
      </div>
    </div>
  </div>
</template>

<script setup>
import "@splidejs/vue-splide/css";
import { Splide, SplideSlide } from "@splidejs/vue-splide";
import { AutoScroll } from "@splidejs/splide-extension-auto-scroll";

const extensions = ref({
  AutoScroll,
});

const Portfolio = ref([
  {
    title: "Embassies and Consulates",
  },
  {
    title: "Official Residences",
  },
  {
    title: "Corporate Headquarters",
  },
  {
    title: "Government Offices",
  },
  {
    title: "Oil and Gas Facilities",
  },
  {
    title: "Nuclear Power Plants",
  },
  {
    title: "Airports and Ports",
  },
]);

const options = ref({
  rewind: true,
  perPage: 3,
  arrows: false,
  pagination: false,
  type: "loop",
  drag: false,
  gap: "11px",

  keyboard: "global",
  autoScroll: {
    speed: 0.5,
    autoStart: false,
  },
  breakpoints: {
    1534: {
      perPage: 3,
    },
    1280: {
      perPage: 5,
    },
    1145: {
      perPage: 4,
    },
    985: {
      perPage: 3,
    },
    661: {
      perPage: 2,
    },
    400: {
      perPage: 1,
    },
  },
});

const splideRef = ref(null);

const startScroll = () => {
  splideRef.value.Components.AutoScroll.play();
};

const stopScroll = () => {
  splideRef.value.Components.AutoScroll.pause();
};

const splideMounted = (e) => {
  splideRef.value = e;
  splideRef.value.Components.AutoScroll.pause();
};
</script>

<style scoped>
.effect {
  background: linear-gradient(
    90deg,
    black 0%,
    rgba(227, 221, 221, 0.112) 45%,
    rgba(227, 221, 221, 0.112) 45%,
    black 90%
  );
}

.bg-card {
  background: linear-gradient(
    97.01deg,
    rgba(255, 255, 255, 0.15) -13.25%,
    rgba(255, 255, 255, 0) 109.79%
  );
}
</style>
