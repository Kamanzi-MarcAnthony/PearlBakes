<template>
    <div class="rose-100">
        <Hero/>

        <div id="favs-section" class="w-screen flex mx-auto pt-16">
        <div class="w-full h-80 flex flex-col items-center mx-auto ">
            <h1 class="text-3xl font-black text-rose-500 ">
                Find Your Favourites from the Cravings corner
            </h1>

            <div class="flex gap-10 justify-between pt-8">
                <FavItems name="custom Bundle" image="/assets/images/custom.svg"/>
                <FavItems name="Butter Croissant" image="/assets/images/butter-croisant.jpg"/>
                <FavItems name="Blueberry Muffins" image="/assets/images/blueberrymuffins.png"/>
                <FavItems name="Cream-Filled Donuts" image="/assets/images/cream-donuts.png"/>
                <FavItems name="Oatmeal Raisin Cookies" image="/assets/images/oatmeal-raisin.png"/>
                <FavItems name="Chocolate Fudge Cake (slice)" image="/assets/images/choco-cake.png"/>
                <FavItems name="Chocolate Muffins" image="/assets/images/choco-muffins.png"/>
            </div>
        </div>
    </div>
    </div>
    
</template>

<script setup>

</script>

<style  scoped>

</style>