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
          {{ $t("tailored-services") }}
        </h3>
        <p class="text-base font-satoshi text-white text-opacity-70">
          {{ $t("expertise") }}
        </p>
      </div>
      <div class="w-full relative space-y-4 effect">
        <Splide
          @splide:mounted="splideMounted"
          :extensions="extensions"
          :options="options"
          @mouseover="startScroll"
          @mouseleave="stopScroll"
        >
          <SplideSlide v-for="(item, index, key) in Services" :key="key">
            <div
              class="py-[16px] h-[72px] w-[72px] bg-[#FFFFFF0D] border border-[#FFFFFF1A] rounded-lg flex relative z-20"
            >
              <div class="m-auto flex flex-col items-center">
                <div>
                  <img
                    :src="item.image"
                    class="object-cover w-[40px] h-[40px]"
                    alt=""
                  />
                </div>
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

const Services = ref([
  {
    image: "/images/thirdsection/Home.svg",
  },
  {
    image: "/images/thirdsection/Camera.svg",
  },
  {
    image: "/images/thirdsection/sun-glasses.svg",
  },
  {
    image: "/images/thirdsection/Star.svg",
  },
  {
    image: "/images/thirdsection/Alert.svg",
  },
  {
    image: "/images/thirdsection/Gps.svg",
  },
  {
    image: "/images/thirdsection/Id.svg",
  },
  {
    image: "/images/thirdsection/Home.svg",
  },
  {
    image: "/images/thirdsection/Home.svg",
  },
]);

const options = ref({
  rewind: true,
  perPage: 7,
  arrows: false,
  pagination: false,
  type: "loop",
  drag: false,
  gap: "11px",
  keyboard: "global",
  autoScroll: {
    speed: 0.5,
    autostart: false,
    // pauseOnHover: true,
  },
  breakpoints: {
    1534: {
      perPage: 7,
    },

    1241: {
      perPage: 12,
    },
    1035: {
      perPage: 10,
    },
    830: {
      perPage: 8,
    },
    644: {
      perPage: 6,
    },
    499: {
      perPage: 4,
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
</style>
