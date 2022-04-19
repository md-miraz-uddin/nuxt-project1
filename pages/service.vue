<template>
  <div class="body_bg">
    <HomeNavbar />
    <ServiceWeProvide />
  </div>
</template>

<script>
import HomeNavbar from '../components/HomeNavbar.vue'
import ServiceWeProvide from '../components/ServiceWeProvide.vue'
export default {
  name: 'ServicePage',
  layout: 'frontend/layout',
  components: {
    HomeNavbar,
    ServiceWeProvide,
  },
  head() {
    return {
      title: 'Service',
    }
  },
}
</script>
