<template>
  <div  class="mt-4  ">
    <div class="hidden flex-col lg:flex md:flex transition-all duration-300 ease-in-out absolute top-0 left-0 w-[260px] pt-[32px] bottom-0">
         <h1 class="font-[400] text-[25px] pl-5 text-black ">LOGO</h1>
        
         
         <!-- this is the content area -->

         <div class="ml-3 mt-16 flex flex-col ">
            <a href="" class=" text-[#757575] capitalize text-[20px] font-bold hover:text-[black] hover:bg-[#dbd9d9] py-2 px-2">shirts</a>
            <a href="" class=" text-[#757575] capitalize text-[20px] font-bold hover:text-[black] hover:bg-[#dbd9d9]  py-2 px-2  ">jackets</a>
            <a href="" class=" text-[#757575] capitalize text-[20px] font-bold hover:text-[black]  hover:bg-[#dbd9d9]  py-2 px-2  ">jeans</a>
            <a href="" class=" text-[#757575] capitalize text-[20px] font-bold hover:text-[black] hover:bg-[#dbd9d9]   py-2 px-2   ">Gymwear</a>
            <a href="" class=" text-[#757575] capitalize text-[20px] font-bold hover:text-[black]  hover:bg-[#dbd9d9]  py-2 px-2  ">shoes</a>

          <!-- contact area -->

          <div class="absolute bottom-0 mb-5 text-[15px] font-[500] ">
              <p class="mb-3">contact</p>
              <p class="mb-3">Newslatter</p>
              <p>Subscribe</p>
            </div>
         </div>
    </div>

    
      <div v-if="isopen" class=" transition-all block lg:hidden md:hidden duration-300 ease-in-out absolute top-0 left-0 w-[260px] bg-white bottom-0">
           <div class="flex justify-between">
             <h1 class="font-[400] text-[25px] mt-10 pl-5 text-black flex   ">LOGO</h1>
             <i @click="$emit('toggle-this', !isopen)" class="fa-solid fa-xmark text-[20px] pr-4 mt-2 p-1 flex  lg:hidden md:hidden hover:bg-gray-400"></i>
           </div>
           <!-- content goes here -->
             <div class="ml-3 mt-16 flex flex-col ">
                <a href="" class=" text-[#757575] capitalize text-[20px] font-bold hover:text-[black] hover:bg-[#dbd9d9] py-2 px-2">shirts</a>
            <a href="" class=" text-[#757575] capitalize text-[20px] font-bold hover:text-[black] hover:bg-[#dbd9d9]  py-2 px-2  ">jackets</a>
            <a href="" class=" text-[#757575] capitalize text-[20px] font-bold hover:text-[black]  hover:bg-[#dbd9d9]  py-2 px-2  ">jeans</a>
            <a href="" class=" text-[#757575] capitalize text-[20px] font-bold hover:text-[black] hover:bg-[#dbd9d9]   py-2 px-2   ">Gymwear</a>
            <a href="" class=" text-[#757575] capitalize text-[20px] font-bold hover:text-[black]  hover:bg-[#dbd9d9]  py-2 px-2  ">shoes</a>
            <!-- contact area -->
            <div class="absolute bottom-0 mb-5 text-[15px] font-[500] ">
              <p class="mb-3">contact</p>
              <p class="mb-3">Newslatter</p>
              <p>Subscribe</p>
            </div>
           </div>
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