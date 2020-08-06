<template>
  <div>
      <nuxt-link to="/styles">
          <v-btn text color="blue">All styles</v-btn>
      </nuxt-link>
      <h1>Textfields</h1>
      
      <v-container style="display: flex">
          <div class="searchBar" style="display: flex">
              <v-text-field filled rounded style="border-radius: 1.5em" placeholder="Search"/>
              <v-btn fab color="blue" style="border-radius: 1.3em; left: -1.5em; "><v-icon>mdi-magnify</v-icon></v-btn>
          </div>

          <div class="searchBar" style="display: flex">
              <v-text-field filled rounded style="border-radius: 1.5em" placeholder="Search"/>
              <v-btn fab color="blue" style="left: -1.5em; "><v-icon>mdi-magnify</v-icon></v-btn>
          </div>

          <div class="searchBar" style="display: flex">
              <v-text-field filled rounded style="border-radius: 0.2em" placeholder="Search"/>
              <v-btn fab color="blue" style="left: -1.5em; "><v-icon>mdi-magnify</v-icon></v-btn>
          </div>

          <div class="searchBar" style="display: flex">
              <v-text-field filled rounded style="border-radius: 0.2em" placeholder="Search"/>
              <v-btn fab outlined color="blue" style="left: 0.3em; border-radius: 0.8em"><v-icon>mdi-magnify</v-icon></v-btn>
          </div>
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