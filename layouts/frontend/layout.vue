<template>
  <v-app>
    <!-- Sizes your content based upon application components -->
    <v-main>
      <!-- Provides the application the proper gutter -->
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>

    <v-footer app>
      <!-- -->
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'layout',
  data() {
    return {
      title: 'Frontend Layout',
    }
  },
}
</script>

<style scoped>
.v-main {
  background-color: #fff;
}
</style>
