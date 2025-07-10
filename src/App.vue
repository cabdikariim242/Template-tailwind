<template>
  <div class="flex flex-col justify-center items-center">  
    <nav class="flex gap-4 mt-4">
      <router-link  class="bg-blue-500 ml-4 py-1 px-4 font-[500] text-[20px]  text-white" to="/">Home</router-link>
      <router-link  class="bg-blue-500 py-1 px-4  text-white font-[500] text-[20px]" to="/about">About</router-link>
    </nav>
    <h1 class="mt-5 font-bold text-2xl text-center text-blue-300">this is the father of vue</h1>

    <router-view/>
  </div>
</template>


<style scoped>
.router-link-exact-active {
  color: blue;
  background-color: red;

}
</style>