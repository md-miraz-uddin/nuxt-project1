<template>
  <v-row>
    <v-col cols="12" sm="4" md="1">
      <nuxt-link to="./"><img src="~/assets/img/inft-bd.png" /></nuxt-link>
    </v-col>
    <v-col cols="12" sm="4" md="9" class="navigation_link">>
      <ul>
        <li><nuxt-link to="./">Home</nuxt-link></li>
        <li><nuxt-link to="./about">About</nuxt-link></li>
        <li><nuxt-link to="./service">Service</nuxt-link></li>
        <li><nuxt-link to="./contact">Contact</nuxt-link></li>
      </ul>
    </v-col>
    <v-col cols="12" sm="4" md="2" class="login_container">
      <nuxt-link to="./backend" class="login_button"
        >Login / Register</nuxt-link
      >
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'HomeNavbar',
}
</script>

<style scoped>
.navigation_link {
	display: flex;
	justify-content: center;
	justify-items: center;
	align-items: center;
	align-content: center;
}

.navigation_link a {
  margin: 0 15px;
  color: #2c2c2c;
  transition: all linear 0.3s;
  font-size: 20px;
}

.navigation_link a:hover {
  margin: 0 15px;
  color: #e12366;
}

.login_container {
  display: flex;
  justify-content: flex-end;
  align-items: center;
  align-content: center;
}
.login_button {
  background-color: #e12366;
  color: #fff;
  padding: 6px 13px;
  border: 1px solid #e12366;
  border-radius: 25px;
}
</style>
