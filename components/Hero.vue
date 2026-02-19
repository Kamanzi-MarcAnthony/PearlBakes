<template>
  <section class="w-screen bg-cover bg-bottom bg-[url(/assets/images/Union.svg)]">
    <div class="flex h-[800px] w-full container mx-auto p-4 justify-between">
        <div class="felx-col justify-center content-center px-auto">
            <h1 class="heading text-8xl tracking-wide font-stretch-condensed">Chef Pearl's Bakes and more..</h1>
            <p class="subheading uppercase font-bold text-3xl text-indigo-700 mt-4">Cakes, Pastries, Bisquits & Bread</p>
        </div>

        <div class=" w-[80%] h-[80%] self-center">
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