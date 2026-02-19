<template>
    <div class="flex flex-col gap-3 justify-center items-center">
        <div 
        class="w-28 h-28 rounded-full outline-rose-400 outline-dotted outline-offset-4  bg-cover bg-center transition-transform duration-300 hover:scale-105"
        :style="bgStyle"></div>
        <h3>{{name}}</h3>
    </div>
</template>

<script>

export default{
    props: {
    name: {
      type: String,
      default: 'Favourite Item'
    },
    image: {
      type: String,
      required: true
    }
  },
  computed: {
    bgStyle() {
      return {
        backgroundImage: `url(${this.image})`
      }
    }
  }
}

</script>

<style lang="scss" scoped>

</style>