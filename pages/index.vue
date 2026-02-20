<template>
    <div class="rose-100 scrollbar-hide">
        <Hero/>

        <div id="favs-section" class="w-screen flex mx-auto pt-16">
            <div class="w-full h-80 flex flex-col items-center mx-auto overflow-hidden">
                <h1 class="md:text-3xl text-2xl text-center font-black text-rose-500 ">
                    Find Your Favourites from the Cravings corner
                </h1>
                <TransitionGroup
                    v-if="showFavs"
                    name="fav"
                    tag="div"
                    class="w-full md:max-w-[80vw] flex gap-10 justify-between pt-8 items-start scroll-smooth snap-start overflow-y-auto snap-x scrollbar-hide"
                >
                    <FavItems
                        v-for="(item, index) in favs"
                        class="text-center gap-3 shrink-0 sm:shrink snap-start"
                        :key="item.name"
                        :name="item.name"
                        :image="item.image"
                        :style="{ animationDelay: `${index * 120}ms` }"
                    />
                </TransitionGroup>
            </div>
        </div>

        <Breakfast/>
    </div>
    
</template>

<script setup>
import { ref, onMounted } from 'vue'

const showFavs = ref(false)

const favs = [
  { name: "custom Bundle", image: "/assets/images/custom.svg"},
  { name: "Butter Croissant", image: "/assets/images/butter-croisant.jpg" },
  { name: "Blueberry Muffins", image: "/assets/images/blueberrymuffins.png" },
  { name: "Cream-Filled Donuts", image: "/assets/images/cream-donuts.png" },
  { name: "Oatmeal Raisin Cookies", image: "/assets/images/oatmeal-raisin.png" },
  { name: "Chocolate Fudge slice", image: "/assets/images/choco-cake.png" },
  { name: "Chocolate Muffins", image: "/assets/images/choco-muffins.png" }
]

onMounted(() => {
  requestAnimationFrame(() => {
    showFavs.value = true
  })
})

</script>

<style >
.fav-enter-active {
  animation: popIn 0.5s ease forwards;
  transition: all 650ms cubic-bezier(0.16, 1, 0.3, 1);
}

.fav-enter-from {
  opacity: 0;
  transform: translateY(20px) scale(0.95);
  filter: blur(4px);
}

.fav-enter-to {
  opacity: 1;
  transform: translateY(0) scale(1);
  filter: blur(0);
}

@keyframes popIn {
  to {
    opacity: 1;
    transform: translateY(0) scale(1);
  }
}


</style>