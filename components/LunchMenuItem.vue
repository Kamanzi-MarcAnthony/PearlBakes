<template>
    <div class="w-[300px] h-[300px] bg-white rounded-lg shadow-lg flex flex-col  border border-black gap-4">
        <div 
        class="w-full h-1/2 p-0 bg-cover bg-center bg-red-700" 
        :style="{ backgroundImage: `url(${image})` }"></div>
        <h3 class="text-xl font-bold">{{name}}</h3>
        
    </div>
</template>

<script>
export default{
    props: {
    name: {
      type: String,
      default: 'Food item'
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