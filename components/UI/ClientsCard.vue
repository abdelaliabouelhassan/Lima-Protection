<template>
  <div
    class="element1 h-full p-[1.5px] rounded-[20px] w-full relative overflow-hidden"
  >
    <img
      src="/images/firstsection/effect.png"
      class="w-full h-full absolute object-cover top-0 right-0"
      alt=""
    />
    <div class="w-full h-full py-[32px] bg-black rounded-[20px] space-y-10">
      <div class="w-full space-y-2 px-[24px] relative z-10">
        <h3 class="text-white font-satoshi font-bold text-2xl">
          Varied clients
        </h3>
        <p class="text-base font-satoshi text-white text-opacity-70">
          From varied backgrounds such as politics, sport, the arts, as well as
          directors and executives of large companies.
        </p>
      </div>
      <div class="w-full relative space-y-4 effect">
        <Splide :extensions="extensions" :options="options">
          <SplideSlide v-for="(item, index, key) in UpperClients" :key="key">
            <div
              class="py-[16px] h-[128px] w-[160px] xl:w-[180px] bg-[#FFFFFF0D] border border-[#FFFFFF1A] rounded-lg flex relative z-20"
            >
              <div class="m-auto flex flex-col items-center">
                <div>
                  <img
                    :src="item.image"
                    class="object-cover w-[60px] h-[60px]"
                    alt=""
                  />
                </div>
                <span class="gradient-text font-satoshi font-medium">{{
                  item.name
                }}</span>
              </div>
            </div>
          </SplideSlide>
        </Splide>
        <Splide :extensions="extensions" :options="options2">
          <SplideSlide v-for="(item, index, key) in LowerClients" :key="key">
            <div
              class="py-[16px] h-[128px] w-[160px] xl:w-[180px] bg-[#FFFFFF0D] border border-[#FFFFFF1A] rounded-lg flex relative z-20"
            >
              <div class="m-auto flex flex-col items-center">
                <div>
                  <img
                    :src="item.image"
                    class="object-cover w-[60px] h-[60px]"
                    alt=""
                  />
                </div>
                <span class="gradient-text font-satoshi font-medium">{{
                  item.name
                }}</span>
              </div>
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

const UpperClients = ref([
  {
    image: "/images/thirdsection/Royalty.svg",
    name: "Royalty",
  },
  {
    image: "/images/thirdsection/Entertainers.svg",
    name: "Entertainers",
  },
  {
    image: "/images/thirdsection/Politicians.svg",
    name: "Politicians",
  },
  {
    image: "/images/thirdsection/Judges.svg",
    name: "Judges",
  },
  {
    image: "/images/thirdsection/Heirs.svg",
    name: "Heirs",
  },
  {
    image: "/images/thirdsection/Philanthropists.svg",
    name: "Philanthropists",
  },
  {
    image: "/images/thirdsection/Eventparticipants.svg",
    name: "Event participants",
  },
]);

const LowerClients = ref([
  {
    image: "/images/thirdsection/Scientists.png",
    name: "Scientists",
  },
  {
    image: "/images/thirdsection/Activist.png",
    name: "Activist",
  },
  {
    image: "/images/thirdsection/SportFigures.png",
    name: "Sport Figures",
  },
  {
    image: "/images/thirdsection/BusinessFigures.png",
    name: "Business Figures",
  },
  {
    image: "/images/thirdsection/Witnesses.png",
    name: "Witnesses",
  },
  {
    image: "/images/thirdsection/Journalists.png",
    name: "Journalists",
  },
  {
    image: "/images/thirdsection/FiguresChildren.png",
    name: "Figures’ Children",
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
    autostart: true,
    pauseOnHover: true,
  },
  breakpoints: {
    1534: {
      perPage: 3,
    },

    1280: {
      perPage: 6,
    },
    1055: {
      perPage: 5,
    },
    880: {
      perPage: 4,
    },
    710: {
      perPage: 3,
    },
    529: {
      perPage: 2,
    },
  },
});

const options2 = ref({
  rewind: true,
  perPage: 3,
  arrows: false,
  pagination: false,
  type: "loop",
  drag: false,
  gap: "11px",
  keyboard: "global",
  autoScroll: {
    speed: -0.5,
    autostart: true,
    pauseOnHover: true,
  },
  breakpoints: {
    1534: {
      perPage: 3,
    },

    1280: {
      perPage: 6,
    },
    1055: {
      perPage: 5,
    },
    880: {
      perPage: 4,
    },
    710: {
      perPage: 3,
    },
    529: {
      perPage: 2,
    },
  },
});
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
</style>
