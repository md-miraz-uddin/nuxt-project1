<template>
  <div class="body_bg">
     <HomeNavbar />
  </div>
</template>

<script>
import HomeNavbar from '../components/HomeNavbar.vue'
export default {
  name: 'IndexPage',
  layout: 'frontend/layout',
  components: {
    HomeNavbar
  },
  head(){
    return{
      title: 'Home'
    }
  }
}
</script>

<style>

</style>
