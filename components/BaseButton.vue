<template>
    <button 
    class="px-6 h-12 rounded-3xl border-black border-b-4 border-t border-r border-l text-black uppercase font-bold transition-all duration-200 ease-out hover:scale-105 hover:shadow-[0_8px_0_0_rgba(0,0,0,1)] active:scale-95 active:translate-y-[2px] active:border-b-2"
    :class="variants[variant]">
        {{label}}
    </button>
    
</template>

<script >
export default {
  props: {
    label: {
      type: String,
      default: 'Click me'
    },
    variant: {
      type: String,
      default: 'yellow'
    }
  },
  computed: {
    variants() {
      return {
        white: 'bg-white hover:bg-white',
        yellow: 'bg-yellow-400 hover:bg-yellow-500',
        pink: 'bg-pink-400 hover:bg-pink-500',
        mint: 'bg-emerald-400 hover:bg-emerald-500',
        orange: 'bg-orange-400 hover:bg-orange-500'
      }
    }
  }
}
</script>

<style lang="scss" scoped>

</style>