<template>
    <div class="text-white bg-rose-400 border-b border-dashed border-white h-24 place-content-center">
        <nav class="flex container mx-auto p-4 justify-between py-4 items-center">
            <NuxtLink to="/" class="font-bold">
                <div class="bg-center bg-center bg-no-repeat bg-bottom bg-[url(/assets/images/Logo.svg)] w-60 h-20"></div>
            </NuxtLink>
            <ul class="flex gap-16">
                <li><NuxtLink to="/cakes">Cakes</NuxtLink></li>
                <li><NuxtLink to="/pastries">Pastries</NuxtLink></li>
                <li><NuxtLink to="/cookies">Cookies & Biscuits</NuxtLink></li>
                <li><NuxtLink to="/breads">Breads</NuxtLink></li>
                <li><NuxtLink to="/chefpearl">About Me</NuxtLink></li>
            </ul>
        </nav>
    </div>
</template>

<script setup>
    
</script>

<style scoped>

</style>