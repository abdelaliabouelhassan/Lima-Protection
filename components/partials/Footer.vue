<template>
  <footer class="w-full py-20 space-y-10 bg-black">
    <!-- <div class="relative z-20">
      <div
        class="w-full max-w-[1180px] mx-auto text-center px-4 pb-4 space-y-8"
      >
        <p class="text-white text-opacity-70 font-satoshi font-medium">
          Organizations we worked with to enhance our services
        </p>
        <div class="w-full flex flex-wrap gap-3 justify-center">
          <a href="#" v-for="n in 7" :key="n">
            <div class="px-[20px] py-[14px] bg-[#101010] rounded-2xl group">
              <div
                class="bg-white bg-opacity-30 w-[113px] h-[16px] group-hover:bg-opacity-100 duration-200"
              ></div>
            </div>
          </a>
        </div>
      </div>
    </div> -->
    <div
      class="flex items-start md:items-center lg:items-start lg:flex-row flex-col justify-center w-full lg:justify-between max-w-[1280px] px-4 xl:px-0 mx-auto"
    >
      <div
        class="max-w-[372px] w-full flex flex-col items-start md:items-center lg:items-start gap-4"
      >
        <div>
          <img
            src="/images/logo.svg"
            class="w-full h-full max-w-[223px] object-cover"
            alt=""
          />
        </div>

        <p class="text-white font-satoshi font-medium">
          {{ $t("company") }}
        </p>

        <div class="flex items-center -space-x-3 md:ml-0 lg:-ml-4 -ml-4">
          <a href="#">
            <img src="/images/facebook.svg" alt="" />
          </a>
          <a href="#">
            <img src="/images/x.svg" alt="" />
          </a>
          <a href="#">
            <img src="/images/linkding.svg" alt="" />
          </a>
          <a href="#">
            <img src="/images/instagram.svg" alt="" />
          </a>
        </div>
      </div>

      <div
        class="flex md:flex-row flex-col items-start md:items-start md:justify-between gap-8"
      >
        <div class="flex flex-col items-start gap-4">
          <h4 class="text-lg font-satoshi text-white font-bold">MENU</h4>
          <a href="#" class="text-white font-satoshi font-medium text-sm">
            {{ $t("about_us") }}
          </a>
          <a href="#" class="text-white font-satoshi font-medium text-sm">
            Services
          </a>
          <!-- <a href="#" class="text-white font-satoshi font-medium text-sm">
            Blog
          </a> -->
          <a href="#" class="text-white font-satoshi font-medium text-sm">
            {{ $t("customers") }}
          </a>
          <a href="#" class="text-white font-satoshi font-medium text-sm">
            {{ $t("contactus") }}
          </a>
        </div>
        <div class="flex flex-col items-start gap-4">
          <h4 class="text-lg font-satoshi text-white font-bold">SERVICES</h4>
          <a href="#" class="text-white font-satoshi font-medium text-sm">
            {{ $t("personalized_risk_assessment") }}
          </a>
          <a href="#" class="text-white font-satoshi font-medium text-sm">
            {{ $t("comprehensive_security_solutions") }}
          </a>
          <a href="#" class="text-white font-satoshi font-medium text-sm">
            {{ $t("proactive_monitoring") }}
          </a>
        </div>
        <div class="flex flex-col items-start gap-4">
          <h4 class="text-lg font-satoshi text-white font-bold uppercase">
            {{ $t("contactus") }}
          </h4>
          <div class="-space-y-4 -mt-4">
            <div class="flex items-center -space-x-3 -space-y-4 gap-2 -ml-5">
              <div>
                <img src="/images/tele.svg" alt="" />
              </div>
              <a
                href="tel:012345678"
                class="text-white font-satoshi font-medium text-sm"
              >
                012345678
              </a>
            </div>
            <div class="flex items-center -space-x-3 -space-y-4 gap-2 -ml-5">
              <div>
                <img src="/images/mail.svg" alt="" />
              </div>
              <a
                href="mailto:abcxyz@gmail.com"
                class="text-white font-satoshi font-medium text-sm"
              >
                abcxyz@gmail.com
              </a>
            </div>
            <div class="flex items-center -space-x-3 -space-y-4 gap-2 -ml-5">
              <div>
                <img src="/images/gpss.svg" alt="" />
              </div>
              <a href="#" class="text-white font-satoshi font-medium text-sm">
                Random address here
              </a>
            </div>
          </div>
          <button
            class="text-black -mt-2 hover:shadow-[0px_0px_25px_rgba(255,255,255,0.5)] font-satoshi font-medium bg-white py-[12px] px-[24px] rounded-full duration-200"
          >
            {{ $t("contactus") }}
          </button>
        </div>
      </div>
    </div>

    <div
      class="max-w-[1280px] mx-auto py-8 border-y border-[#FFFFFF4D] px-4 xl:px-0"
    >
      <p class="text-white font-medium font-satoshi text-sm text-center">
        CNAPS AUT-077-2123-04-26-20240925398 <br />
        Article L. 612-14 du Code de la sécurité intérieure : « L'autorisation
        d'exploitation ne confère aucune prérogative de puissance publique à
        l'entreprise ou aux personnes qui en bénéficient.
      </p>
    </div>

    <div
      class="max-w-[1280px] mx-auto flex items-center md:flex-row flex-col gap-4 md:justify-between px-4 xl:px-0"
    >
      <p class="text-white font-medium font-satoshi text-sm">
        © {{ new Date().getFullYear() }} {{ $t("copyright") }}
      </p>

      <div class="flex items-center gap-4">
        <a
          href="#"
          class="text-white font-medium font-satoshi text-sm underline"
          >{{ $t("cookies") }}</a
        >
        <router-link
          to="/privacy-policy"
          class="text-white font-medium font-satoshi text-sm underline"
          >{{ $t("privacy") }}</router-link
        >
        <router-link
          to="/terms"
          class="text-white font-medium font-satoshi text-sm underline"
          >{{ $t("terms") }}</router-link
        >
        <a
          href="#"
          class="text-white font-medium font-satoshi text-sm underline"
          >{{ $t("sitemap") }}</a
        >
      </div>
    </div>
  </footer>
</template>
