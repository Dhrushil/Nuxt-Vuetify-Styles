<template>
  <div class="gmail">
    <nuxt-link to="/styles">
      <v-btn text color="blue">All styles</v-btn>
    </nuxt-link>
    <h1>Gmail API</h1>
    <v-container>
        <v-btn @click="Location">Location</v-btn>
        <h1>{{address}}</h1>

    </v-container>
  </div>
</template>

<script>
export default {
    data() {
        return {
            address: ""
        };
    },
  methods: {
    Location() {
      navigator.geolocation.getCurrentPosition(
        position => {
          this.address = position.coords.latitude + " " + position.coords.longitude
        },
        error => {
          console.log(error.message);
        }
      );
    }
  },
  mounted() {
    this.Location();
  }
};
</script>
<style>
</style>