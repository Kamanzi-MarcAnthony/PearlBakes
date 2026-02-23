<template>
    <div class="w-[300px] h-[300px] bg-white flex flex-col gap-2 justify-between items-center">
        <div 
        class="w-full h-1/2 p-0 bg-cover bg-center rounded-tl-3xl rounded-br-3xl hover:scale-105 transition-transform duration-300" 
        :style="{ backgroundImage: `url(${image})` }"></div>
        <h3 class="text-xl font-bold">{{name}}</h3>
        <p>{{description}}</p>
        <NuxtLink to="/" class=" font-medium hover:text-rose-400 underline decoration-wavy decoration-1 rounded-lg"> Place Order</NuxtLink>
        
    </div>
</template>
 
<script>
export default{
    props: {
    name: {
      type: String,
      default: 'Food item'
    },
    description: {
      type: String,
      default: 'Delicious food item description goes here.'
    },
    image: {
      type: String,
      required: true
    }
  }
}

</script>

<style scoped>

</style>