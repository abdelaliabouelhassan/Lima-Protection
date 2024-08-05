<template>
  <section class="sm:-space-y-14 pb-24">
    <div class="w-full relative sm:-space-y-20">
      <div class="sm:block hidden">
        <img src="/images/hero-bg.png" class="w-full sm:h-[1025px]" alt="" />
      </div>

      <div
        class="sm:absolute pt-14 sm:pt-0 bottom-14 sm:bottom-64 md:bottom-48 left-0 w-full"
      >
        <div class="flex flex-col items-center sm:-space-y-36">
          <div class="sm:block hidden">
            <img
              src="/images/Mask.png"
              class="w-full lg:w-[456px] h-full object-cover"
              alt=""
            />
          </div>
          <div class="sm:hidden">
            <img
              src="/images/mask-mobile.png"
              class="w-full object-cover h-[450px]"
              alt=""
            />
          </div>

          <div
            class="max-w-[714px] text-center space-y-6 flex flex-col items-center px-4 md:px-0 -mt-[10rem]"
          >
            <h1
              class="font-bold font-satoshi text-white text-3xl md:text-5xl leading-normal md:leading-[63px]"
            >
              We offer Exclusive, Safe & Secured Protection
            </h1>
            <p
              class="text-white text-opacity-70 font-normal max-w-[612px] text-center"
            >
              Our security company established in the Paris region,
              <span class="font-bold text-white">Lima Protection</span>,
              provides private aid and close security missions both in France
              and abroad.
            </p>

            <div class="pt-6">
              <a
                href="https://ax6hl0zetxi.typeform.com/to/ehMKwuTo"
                target="_blank"
              >
                <button class="element rounded-full p-px group duration-300">
                  <div
                    class="rounded-full py-[12px] px-[20px] text-white font-satoshi font-medium bg-black duration-300 bg-gradient-to-br group-hover:from-[#ffffff80] group-hover:to-[#00000001] from-[#ffffff30] from-[9.11%] to-[#00000001] to-[76.61%]"
                  >
                    Hire us
                  </div>
                </button>
              </a>
            </div>
          </div>
        </div>
      </div>
      <div class="w-full hidden">
        <div class="w-full flex justify-center">
          <div class="flex items-center flex-wrap justify-center gap-2">
            <span class="text-white text-opacity-70 font-satoshi font-medium"
              >Regulated by</span
            >
            <div class="h-[22px] w-[64px]">
              <img
                src="/images/head.png"
                class="w-full h-full object-cover"
                alt=""
              />
            </div>
            <span class="text-white font-medium font-satoshi"
              >the French Ministry for Interior</span
            >
          </div>
        </div>
      </div>
    </div>

    <div class="w-full flex flex-col items-center gap-8 pt-14 sm:pt-0">
      <span class="text-white text-opacity-70 font-medium font-satoshi"
        >They are writing about us:</span
      >

      <div
        class="w-full flex flex-wrap gap-3 max-w-[1180px] mx-auto px-4 justify-center"
      >
        <a href="#" v-for="n in 7" :key="n">
          <div class="px-[20px] py-[14px] bg-[#101010] rounded-2xl group">
            <div
              class="bg-white bg-opacity-30 w-[113px] h-[16px] group-hover:bg-opacity-100 duration-200"
            ></div>
          </div>
        </a>
      </div>
    </div>
  </section>
</template>
