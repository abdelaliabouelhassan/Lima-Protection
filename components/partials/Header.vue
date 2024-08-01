<template>
    <header class=" w-full">
        <div class=" w-full max-w-[1313px] mx-auto flex items-center justify-between px-4 pb-4 pt-8">
            <div>
                <img src="/images/logo.svg" class=" w-full h-full object-cover" alt="">
            </div>

           <div class="element rounded-full  p-px">
             <div class=" bg-black rounded-full   py-[12px] px-[32px] flex items-center justify-between gap-9 ">
                <a href="#" class=" font-satoshi text-white text-opacity-50 text-base font-normal hover:text-opacity-80 duration-200">
                    About us
                </a>
                 <a href="#" class=" font-satoshi text-white text-opacity-50 text-base font-normal hover:text-opacity-80 duration-200">
                    Blog
                </a>
                 <a href="#" class=" font-satoshi text-white text-opacity-50 text-base font-normal hover:text-opacity-80 duration-200">
                    Customers
                </a>
                 <a href="#" class=" font-satoshi text-white text-opacity-50 text-base font-normal hover:text-opacity-80 duration-200">
                    Resources
                </a>

                <div class=" h-[26px] w-px bg-white bg-opacity-20"></div>

                <div class=" relative">
                    <div class=" flex items-center gap-2 cursor-pointer" @click="open = !open">
                        <div>
                            <img src="/images/uk.png" class=" w-full h-full object-cover" alt="">
                        </div>
                        <span class=" font-satoshi text-white">EN</span>
                        <div>
                              <svg width="12" height="6" viewBox="0 0 12 6" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path d="M10.5 0.75L6 5.25L1.5 0.749999" stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
                              </svg>
                        </div>
                    </div>

                    <div class=" absolute left-0 top-8 p-2 bg-black w-full flex flex-col gap-2 rounded" v-if="open">
                        <div class=" flex items-center gap-2 cursor-pointer" v-for=" n in 2" :key="n">
                            <div>
                                <img src="/images/uk.png" class=" w-full h-full object-cover" alt="">
                            </div>
                            <span class=" font-satoshi text-white">FR</span>
                        
                        </div>
                    </div>
                </div>
            </div>
           </div>


           <div class=" flex items-center gap-4">
            <a href="#" class=" text-white text-opacity-60 font-satoshi hover:text-opacity-80 duration-200">Apply</a>
            <button class=" text-black font-satoshi font-medium bg-white py-[12px] px-[24px] rounded-full hover:bg-opacity-80 duration-200">Hire us</button>
           </div>
        </div>
    </header>
</template>

<script setup>
 const open = ref(false)
</script>

<style scoped>




</style>