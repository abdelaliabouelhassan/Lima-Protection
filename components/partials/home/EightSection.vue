<template>
  <section class="w-full p-10 space-y-14 relative overflow-hidden px-4 xl:px-0">
    <div
      style="
        background: linear-gradient(
          180deg,
          rgba(255, 255, 255, 0.25) -9.55%,
          rgba(255, 255, 255, 0) 85.45%
        );
      "
      class="relative h-[827px] overflow-hidden max-w-[1280px] w-full mx-auto p-[1.5px] rounded-t-[32px]"
    >
      <div class="effect-bg rounded-t-[32px]">
        <div
          class="flex flex-col items-center gap-6 px-4 text-center z-10 relative pt-10"
        >
          <div>
            <img
              src="/images/quote.svg"
              class="w-full h-full object-cover"
              alt=""
            />
          </div>

          <h3 class="text-white font-satoshi font-bold text-4xl">
            Listen to our customers
          </h3>
          <p
            class="font-satoshi font-normal text-base text-white text-opacity-60"
          >
            We prospect qualified candidates to be part of our elite protection
            team
          </p>
        </div>

        <div class="w-full pt-20 space-y-5 relative group">
          <div
            class="w-full h-full absolute top-0 left-0 card-effect z-40"
          ></div>
          <Splide
            :extensions="extensions"
            :options="options"
            class="relative group-hover:z-50"
          >
            <SplideSlide v-for="n in 10" :key="n">
              <ReviewCard />
            </SplideSlide>
          </Splide>
          <Splide
            :extensions="extensions"
            :options="options2"
            class="relative group-hover:z-50"
          >
            <SplideSlide v-for="n in 10" :key="n">
              <ReviewCard />
            </SplideSlide>
          </Splide>
          <Splide :extensions="extensions" :options="options">
            <SplideSlide v-for="n in 10" :key="n">
              <ReviewCard />
            </SplideSlide>
          </Splide>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import ReviewCard from "@/components/UI/ReviewCard.vue";
import "@splidejs/vue-splide/css";
import { Splide, SplideSlide } from "@splidejs/vue-splide";
import { AutoScroll } from "@splidejs/splide-extension-auto-scroll";

const extensions = ref({
  AutoScroll,
});

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

    657: {
      perPage: 2,
    },
    467: {
      perPage: 1,
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

    657: {
      perPage: 2,
    },
    467: {
      perPage: 1,
    },
  },
});
</script>

<style scoped>
.effect-bg {
  background: radial-gradient(
    36.38% 36.38% at 50% 0%,
    #2d2d2d 0%,
    #000000 100%
  );
}

.card-effect {
  background: linear-gradient(
    0deg,
    #000000 0%,
    rgba(0, 0, 0, 0.7) 40.37%,
    rgba(115, 115, 115, 0) 100%
  );
}
</style>
