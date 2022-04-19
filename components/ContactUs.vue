<template>
  <div>
    <v-row>
      <v-col cols="12" sm="12" md="7" class="mx-auto">
        <h3>let's have a Chat</h3>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="12" sm="7" class="mx-auto">
        <v-row>
          <v-col cols="12" sm="5">
            <div>
              <img src="~/assets/img/contact_us.png" />
            </div>
          </v-col>
          <v-col cols="12" sm="7">
            <div class="contact-form">
              <!-- Shapes -->

              <!-- Shapes -->
              <div class="text">
                <h5>Get In Touch</h5>
                <h2>
                  We Provide Best Services.
                  <br />
                  Need Help?
                </h2>
              </div>

              <form>
                <div>
                    <input type="text" placeholder="Email Address">
                </div>
                <div>
                    <textarea name="" id="" rows="4"></textarea>
                </div>

                <v-btn class="mr-4"> submit </v-btn>
              </form>
            </div>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: 'ContactUs',
}
</script>

<style scoped>
* {
  color: #2c2c2c;
  font-family: 'Roboto', sans-serif;
}

.row:nth-child(1) {
  margin-bottom: 30px;
}

.row:nth-child(2) {
  height: 100vh;
}

h3 {
  margin: 50px 0 15px 0;
  text-align: center;
  font-size: 40px;
}

p {
  text-align: center;
  font-size: 18px;
  padding: 50px;
  color: #545b63;
}

input, textarea {
	width: 100%;
	border: 1px solid #2c2c2c;
	padding: 15px;
	margin-top: 10px;
}

textarea {
    resize: none;
    margin-bottom: 15px;
}
</style>
