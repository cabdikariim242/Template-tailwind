<template>
  <div class="flex flex-col justify-center items-center">  
   <navbar/>
    <sidebar/>
  </div>
</template>


<script>
import sidebar from './components/sidebar.vue'
import navbar from './components/navbar.vue'
export default {
  components: {sidebar, navbar}
}
</script>

<style scoped>
.router-link-exact-active {
  color: blue;
  background-color: red;

}
</style>