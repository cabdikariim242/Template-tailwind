<template>
   
  <div class="flex flex-col justify-center  items-center">
   <navbar :isopen="isopen" @toggle-this="toggle" />
<sidebar :isopen="isopen" @toggle-this="toggle" />
<content/>
  </div>
</template>


<script>
import sidebar from './components/sidebar.vue'
import navbar from './components/navbar.vue'
import content from './components/content.vue'
export default {
  components: {sidebar, navbar,content},
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
.router-link-exact-active {
  color: blue;
  background-color: red;

}
</style>
