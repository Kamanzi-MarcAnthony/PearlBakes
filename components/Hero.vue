<template>
  <section class="w-screen bg-cover bg-bottom bg-[url(/assets/images/Union.svg)]">
    <div class="flex flex-col md:flex-row h-[85vh] md:min-h-[80vh] w-full container mx-auto p-4 justify-between">
      <!-- Text -->
        <div class="flex-col justify-center content-center text-center md:text-left max-w-xl">
            <h1 class="heading text-4xl sm:text-5xl md:text-7xl lg:text-8xl tracking-wide leading-tight">Chef Pearl's Bakes and more..</h1>
            <p class="subheading uppercase font-bold text-xl sm:text-xl md:text-3xl text-indigo-700 mt-4">Cakes, Pastries, Bisquits & Bread</p>
            <!-- buttons -->
            <div class="mt-8 flex flex-col sm:flex-row gap-4 sm:gap-6 justify-center md:justify-start">
              <NuxtLink>
                <BaseButton label="Explore my menus"/>
              </NuxtLink>

              <NuxtLink>
                <BaseButton label="View my Catalog" variant="white"/>
              </NuxtLink>
            </div>
        </div>

        <!-- hero img -->
        <div class="w-full md:w-[80%] h-full sm:h-[100%] md:h-[100%] self-center overflow-hidden">
            <div class="w-full h-full bg-cover bg-center masked-img bg-[url(/assets/images/chef.png)] transition-all duration-700 ease-out hover:scale-110 hover:bg-top"></div>
        </div>
    </div>
  </section>
</template>

<script setup>

</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Bagel+Fat+One&family=DynaPuff:wght@400..700&family=Rubik+Dirt&family=Story+Script&display=swap');


/* global.css */
.masked-img {
  -webkit-mask-image: linear-gradient(to bottom, black 20%, transparent 90%);
  mask-image: linear-gradient(to bottom, black 50%, transparent 90%);
}

.heading{
   font-family: "Bagel Fat One", system-ui;
    font-weight: 400;
    font-style: normal;
    color: white;
}

.subheading{
    font-family: "DynaPuff", system-ui;
    font-optical-sizing: auto;
    font-weight: 600;
    font-style: normal;
    font-variation-settings:
    "wdth" 100;
}
</style>