<template>
  <div class="icons">
      <nuxt-link to="/styles">
          <v-btn text color="blue"> All styles</v-btn>
      </nuxt-link>
      <h1>Icons</h1>
      <v-container>
          <v-card width="20%">
              <v-container> 
              <v-btn fab color="#fb3958" style="border-radius: 1.4em"> 
              <v-icon x-large>mdi-youtube</v-icon>
              </v-btn>
              <v-btn fab color="blue" style="border-radius: 1.4em"> 
              <v-icon x-large>mdi-github</v-icon>
              </v-btn>
              <v-btn fab color="#ff7700" style="border-radius: 1.4em"> 
              <v-icon x-large>mdi-soundcloud</v-icon>
              </v-btn>
              </v-container>
          </v-card>
      </v-container>
  </div>
</template>

<script>
export default {

}
</script>

<style>
h1 {
    text-align: center;
}
</style>