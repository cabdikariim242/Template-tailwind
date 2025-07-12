<template>
  <div class="flex flex-col w-full ">
    <div
      class="flex w-full h-20 lg:hidden md:hidden bg-black text-white justify-between items-center"
    >
      <h1 class="font-[400] pl-5 text-[25px]">LOGO</h1>
      <i @click="$emit('toggle-this', !isopen)" class="fa-solid fa-bars text-[25px] hover:bg-gray-500 p-[28px]"></i>
    </div>

    <!-- content section -->
    <div  class="flex lg:ml-[270px] md:ml-[270px] transition-all duration-300 ease-in-out ml-5 tran justify-between mx-5 mt-6 ">
      <div>
        <h1 class="text-[30px] ">Jeans</h1>
      </div>

      <div class="">
        <i  class="fa-solid fa-cart-shopping text-[20px] mr-5"></i>
        <i class="fa-solid fa-magnifying-glass text-[20px]" style="color: #000000"></i>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['isopen']
}
</script>