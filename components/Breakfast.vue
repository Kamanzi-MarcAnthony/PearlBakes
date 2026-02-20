<template>
  <section class="w-screen h-[800px] bg-yellow-200 flex place-content-center items-center">
    <div class="md:w-[90%] md:h-[90%] w-[90%] h-[90%] md:bg-white overflow-hidden flex flex-col md:flex-row rounded-2xl">

        <div class="w-1/2 h-full hidden md:block flex ">
            <div class=" w-[80%] h-[90%] bg-[url(/assets/images/breakfast.svg)] bg-contain bg-no-repeat bg-center justify-self-center animate-float mt-8"></div>
        </div>

        <div class="md:w-1/2 pb-16  bg-right  bg-[url(/assets/images/Union2.svg)] bg-no-repeat bg-cover flex items-center justify-center">
            <div class="flex-col justify-center content-center text-center md:text-left max-w-xl ml-4">
                <div class=" md:hidden sm:block w-[350px] h-[380px] bg-[url(/assets/images/breakfast.svg)] animate-float bg-cover bg-center justify-self-center mb-2"></div>
                <h1 class="heading text-4xl sm:text-5xl md:text-5xl lg:text-5xl tracking-wide leading-tight">My Hot Breakfast Combos Made Fresh, Daily</h1>
                <p class="subheading uppercase font-bold text-lg sm:text-xl md:text-3xl text-indigo-700 mt-4">Freshly baked breakfast & coffee-ready combos</p>
            <!-- buttons -->
            <div class="mt-8 sm:flex-row gap-4 sm:gap-6 justify-center md:justify-start">
              <NuxtLink>
                <BaseButton label="Order Your Breakfast"/>
              </NuxtLink>
            </div>
        </div>
        </div>
    </div>
    
  </section>
</template>

<script setup>

</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Bagel+Fat+One&family=DynaPuff:wght@400..700&family=Rubik+Dirt&family=Story+Script&display=swap');


@keyframes float {
  0%, 100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-10px);
  }
}

.animate-float {
  animation: float 3.5s ease-in-out infinite;
}

</style>