<template>
    <button class="px-6 h-12 bg-yellow-400 rounded-3xl border-black border-b-4 border-t border-r border-l text-black transition-all duration-200 ease-out hover:scale-105 hover:shadow-[0_8px_0_0_rgba(0,0,0,1)] active:scale-95 active:translate-y-[2px] active:border-b-2">
        {{label}}
    </button>
    
</template>

<script>
export default{
    props: ['label']
}

</script>

<style lang="scss" scoped>

</style>