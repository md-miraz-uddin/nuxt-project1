<template>
  <div class="body_bg">
    <HomeNavbar />
    <AboutUs />
  </div>
</template>

<script>
import HomeNavbar from '../components/HomeNavbar.vue'
import AboutUs from '../components/AboutUs.vue'
export default {
  name: 'AboutPage',
  layout: 'frontend/layout',
  components: {
    HomeNavbar,
    AboutUs,
  },
  head() {
    return {
      title: 'About',
    }
  },
}
</script>

