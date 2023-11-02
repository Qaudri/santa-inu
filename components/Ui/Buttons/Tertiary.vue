<template>
  <div>
    <button @click="emitclicked" class="font-normal text-sm xl:text-base 2xl:text-lg hover:text-primary ease-in-out duration-300 border-b border-transparent hover:border-primary select-none text-left outline-none focus:outline-none focus:border-primary" :class="white_text ? 'text-white' : 'text-accent'">
      <slot />
    </button>
  </div>
</template>

<script>
export default {
  props: {
    white_text: Boolean
  },
  methods: {
    emitclicked(){
      this.$emit("clicked")
    }
  }
}
</script>

<style>

</style>