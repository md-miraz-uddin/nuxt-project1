<template>
  <div class="body_bg">
    <HomeNavbar />
    <ContactUs />
  </div>
</template>

<script>
import HomeNavbar from '../components/HomeNavbar.vue'
import ContactUs from '../components/ContactUs.vue'
export default {
  name: 'ContactPage',
  layout: 'frontend/layout',
  components: {
    HomeNavbar,
    ContactUs,
  },
  head() {
    return {
      title: 'Contact',
    }
  },
}
</script>
