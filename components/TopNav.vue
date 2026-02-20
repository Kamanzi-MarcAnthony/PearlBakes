<template>
    <div class="text-white bg-rose-400 border-b border-dashed border-white h-24 place-content-center">
        <nav class="flex container mx-auto p-4 justify-between py-4 items-center">
            <!-- logo -->
            <NuxtLink to="/" class="font-bold">
                <div class="bg-center bg-center bg-no-repeat bg-bottom bg-[url(/assets/images/Logo.svg)] w-40 md:w-60 h-16 md:h-20"></div>
            </NuxtLink>
            <!-- Desktop nav -->
            <ul class="hidden md:flex gap-16">
                <li><NuxtLink to="/cakes">Cakes</NuxtLink></li>
                <li><NuxtLink to="/pastries">Pastries</NuxtLink></li>
                <li><NuxtLink to="/cookies">Cookies & Biscuits</NuxtLink></li>
                <li><NuxtLink to="/breads">Breads</NuxtLink></li>
                <li><NuxtLink to="/chefpearl">About Me</NuxtLink></li>
            </ul>
            <!-- Desktop CTA -->
             <div class="hidden md:block">
                <NuxtLink>
                    <BaseButton label="Place your Order" variant="yellow"/>
                </NuxtLink>
             </div>

             <!-- Mobile Hamburger -->
            <button class="md:hidden w-10 h-10 bg-no-repeat bg-center bg-contain hover:scale-105 transition-transform bg-[url(/assets/images/fastfood_24dp_E3E3E3_FILL0_wght400_GRAD0_opsz24.svg)]"></button>
        </nav>
    </div>
</template>

<script setup>
    
</script>

<style scoped>

</style>