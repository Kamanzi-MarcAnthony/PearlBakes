<template>
    <div class="w-screen p-4 flex flex-col justify-center mt-8">
        <div class=" w-full md:w-[80%] md:justify-between gap-4 flex flex-col md:flex-row mx-auto">
            <div>
                <h1 class="heading text-center text-4xl sm:text-5xl md:text-5xl lg:text-5xl tracking-wide leading-tight">My Hot Lunch Combos Made Fresh, Daily</h1>
                <p class="subheading text-indigo-700 text-center md:text-left text-lg mt-4">Curated lunch meals, crafted for serious flavor lovers.</p>
            </div>
            <BaseButton
                class="hidden md:block"
                label="See Full Lunch Menu"
            />
        </div>

        <div class="flex flex-col p-2 md:flex-row  h-1/2 w-full place-content-center items-center justify-center gap-10 md:gap-20 mt-8">
            <LunchMenuItem 
                v-for="(item, index) in lunches" 
                :key="item.name" 
                :name="item.name"
                :description="item.description" 
                :image="item.image" 
                :style="{ animationDelay: `${index * 120}ms` }" 
            />
        </div>
    </div>
</template>

<script setup>

import { ref, onMounted } from 'vue'
const   showLunches = ref(false)

const lunches = [
    {name: "Oven Baked Whole Fish", 
    description:"Juicy whole fish oven-baked with herbs and mild spices — fresh & flavorful", 
    image: "/assets/images/custom.svg"},

    {name: "Slow-Braised Goat Stew",
    description:"Rich and hearty stew slow-braised with aromatic spices and tender goat meat",
    image: "/assets/images/custom.svg"},

    { name: "Creamy Groundnut Chicken",
    description:"Comforting peanut sauce with tender chicken",
    image: "/assets/images/custom.svg"},

    { name: "Slow-Braised Goat Stew",
    description:"Rich and hearty stew slow-braised with aromatic spices and tender goat meat",
    image: "/assets/images/custom.svg"}
    
]


onMounted(() => {
  requestAnimationFrame(() => {
    showLunches.value = true
  })
})

</script>

<style scoped>


</style>