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

        <div class="flex flex-col p-2 md:flex-row  h-1/2 w-full place-content-center items-center justify-center gap-4 mt-8">
            <LunchMenuItem/>
        </div>


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
  }
}

</script>

<style scoped>


</style>