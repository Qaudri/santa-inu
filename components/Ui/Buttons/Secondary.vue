<template>
  <div>
    <button @click="emitclicked()" class="py-2 px-5 text-accent border-accent focus:text-white hover:text-white border font-medium text-base 2xl:text-lg justify-center duration-300 ease-in-out rounded-md outline-none focus:outline-none" :class="[flexdisplay ? 'flex w-full' : 'block w-fit', standout ? 'bg-primary  border-primary hover:bg-secondary focus:bg-secondary': 'bg-transparent hover:bg-primary focus:bg-primary hover:border-primary focus:border-primary']">
      <slot />
    </button>
  </div>
</template>

<script>
export default {
  props: {
    flexdisplay: Boolean,
    standout: Boolean
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