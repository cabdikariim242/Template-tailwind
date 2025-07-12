<template>
   
  <div class="flex flex-col justify-center  items-center">
   <navbar :isopen="isopen" @toggle-this="toggle" />
<sidebar :isopen="isopen" @toggle-this="toggle" />

  </div>
</template>


<script>
import sidebar from './components/sidebar.vue'
import navbar from './components/navbar.vue'
export default {
  components: {sidebar, navbar},
  data(){
    return{
     isopen: true
  }},
 methods: {
  toggle(value) {
    this.isopen = value
  }
}
}

</script>

<style >
body{
}
.router-link-exact-active {
  color: blue;
  background-color: red;

}
</style>
