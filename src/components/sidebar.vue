<template>
  <div  class="mt-4  ">
<div class="hidden lg:flex md:flex  justify-between transition-all duration-300 ease-in-out absolute top-0 left-0 w-[300px] pt-[32px] bottom-0 bg-blue-800">
         <h1 class="font-[400] text-[25px] pl-5 text-white ">LOGO</h1>
         
    </div>

    <div v-if="isopen" class="flex justify-between transition-all duration-300 ease-in-out absolute top-0 left-0 w-[300px] pt-[32px] bottom-0 bg-blue-800">
         <h1 class="font-[400] text-[25px] pl-5 text-white ">LOGO</h1>
         <i @click="$emit('toggle-this', !isopen)" class="fa-solid fa-xmark text-[20px] pr-4 flex  lg:hidden md:hidden"></i>
    </div>
  </div>
</template>

<script>
export default {
  
  props: ['isopen'],
  //  methods:{
  //   toggle(){
     
  //     this.$emit('toggle-this' , this.isopen)
  //   }
  //  }
  }

</script>