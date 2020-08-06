<template>
  <div class="comments">
    <nuxt-link to="/styles">
      <v-btn text color="blue">All styles</v-btn>
    </nuxt-link>
    <h1>Comments</h1>

    <v-container>
      <v-card style="border-radius: 0.7em">
        <v-container>
          <div class="youtube-meta" style="display: flex">
            <iframe
              width="250%"
              height="600"
              src="https://www.youtube.com/embed/tLNBvwLvA2o"
              style="border-radius: 1em"
            ></iframe>
            <v-container>
              <h2>Wide Melonpan walking but he's always in frame</h2>
              <h5>881,271 views • Jun 12, 2015</h5>
            </v-container>
          </div>
          <h2 style="text-align: center;">Comments</h2>
          <div class="comments_sec">
            <v-card>
              <v-container style="display: flex">
                <v-avatar color="indigo" size="36"></v-avatar>
                <v-container>
                  <h3>User_name</h3>
                  <h5>User Comments</h5>
                </v-container>
              </v-container>
              <v-btn fab x-small style="top: 0.5em; border-radius: 1em" color="#0D47A1">
                <v-icon>mdi-thumb-up</v-icon>
              </v-btn>
              <v-btn fab x-small style="top: 0.5em; border-radius: 1em" color="#FF1744">
                <v-icon>mdi-thumb-down</v-icon>
              </v-btn>
              <v-btn text @click="expand = !expand">Reply</v-btn>
            </v-card>
            <v-expand-transition>
              <v-card v-show="expand" width="80%" class="mx-auto">
                <v-textarea name="input-7-4" label="Reply" auto-grow></v-textarea>
                <v-btn fab small style="top: 0.5em; border-radius: 1em" color="#E53935" @click="expand = false">
                  <v-icon>mdi-cancel</v-icon>
                </v-btn>
                <v-btn fab small style="top: 0.5em; border-radius: 1em" color="#00C853">
                  <v-icon>mdi-send</v-icon>
                </v-btn>
              </v-card>
            </v-expand-transition>
          </div>
        </v-container>
      </v-card>
    </v-container>
  </div>
</template>



<style>
h1 {
  text-align: center;
}
</style>

<script>
export default {
  data: () => ({
    expand: false
  })
};
</script>