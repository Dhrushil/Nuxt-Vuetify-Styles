<template>
  <div>
      <nuxt-link to="/styles">
    <v-btn text color="blue"> All styles </v-btn>
      </nuxt-link>
    <h1>Cards</h1>
    <v-container style="display:flex">
      <v-card width="20%" style="border-radius: 2.5em" class="ms-10">
        <v-container>
          <v-btn
            style="position: absolute; z-index: 5; border-radius: 20px; height: 63px; left: -2em; top: -1em;"
          >
            <v-icon color="red">mdi-heart</v-icon>
          </v-btn>
          <v-img
            max-height="100%"
            max-width="100%"
            fit
            src="https://cdn.dribbble.com/users/747805/screenshots/9756616/media/66d965176548313bd8f8225fe9a2fea9.jpg"
            style="border-radius: 1.5em;"
          ></v-img>
          <div>
            <v-card-title>Vuetify 2</v-card-title>
            <v-card-subtitle>Framework</v-card-subtitle>
          </div>
        </v-container>
      </v-card>

        
      <v-card width="20%" style="border-radius: 2.5em" class="ms-10" >
        <v-container style="z-index: 5">
            <v-btn
            style="position: absolute; z-index: 5; border-radius: 20px; height: 63px; right: -2em; top: -1em;"
          ><v-icon color="green">mdi-share</v-icon></v-btn>
          <v-img
            max-height="100%"
            max-width="100%"
            fit
            src="https://cdn.dribbble.com/users/518045/screenshots/11416007/media/6efe26d03123144ca77e762a0853a4e1.png"
            style="border-radius: 1.5em;"
          ></v-img>
          <div style="top: -1.7em; position: relative">
            <v-btn small style="border-radius: 1em; left: 2em" fab>
              <v-icon color="red">mdi-heart</v-icon>
            </v-btn>
              <v-btn small style="border-radius: 1em; left: 2em" fab @click="expand = !expand">
                <v-icon color="blue">mdi-comment</v-icon>
              </v-btn>
            <v-card-title>Get Started</v-card-title>
            <v-card-subtitle>Vuetify 2 is an open source framework and you can even help in simple details</v-card-subtitle>
            <div style="display: flex;">
              <v-text-field filled rounded dense style="border-radius: 0.8em; width: 50%;" placeholder="comment"></v-text-field>&nbsp;
              <v-btn small style="border-radius: 1em;" color="purple" fab>
                <v-icon color="white">mdi-send</v-icon>
              </v-btn>
            </div>
          </div>
        </v-container>
        <v-expand-x-transition>
        <v-card
          v-show="expand"
          height="90%"
          width="100%"
          class="mx-auto"
          style="position: absolute; top: 5%; left: 98%; border-radius: 2em; border-top-left-radius: 0; border-bottom-left-radius: 0;"
        ></v-card>
      </v-expand-x-transition>
      </v-card>

      <v-card width="20%" style="border-radius: 2.5em" class="ms-10" >
        <v-container style="z-index: 5">
            <v-btn
            style="position: absolute; z-index: 5; border-radius: 20px; height: 63px; right: -2em; top: -1em;"
          ><v-icon color="green">mdi-share</v-icon></v-btn>
         <iframe
              max-width="100%"
              height="200"
              src="https://www.youtube.com/embed/tLNBvwLvA2o"
              style="border-radius: 1em"
            ></iframe>
          <div style="top: -1.7em; position: relative">
            <v-btn small style="border-radius: 1em; left: 2em" fab>
              <v-icon color="red">mdi-heart</v-icon>
            </v-btn>
              <v-btn small style="border-radius: 1em; left: 2em" fab @click="expand2 = !expand2">
                <v-icon color="blue">mdi-comment</v-icon>
              </v-btn>
            <v-card-title>Get Started</v-card-title>
            <v-card-subtitle>Vuetify 2 is an open source framework and you can even help in simple details</v-card-subtitle>
            <div style="display: flex;">
              <v-text-field filled rounded dense style="border-radius: 0.8em; width: 50%;" placeholder="comment"></v-text-field>&nbsp;
              <v-btn small style="border-radius: 1em;" color="purple" fab>
                <v-icon color="white">mdi-send</v-icon>
              </v-btn>
            </div>
          </div>
        </v-container>
        <v-expand-x-transition>
        <v-card
          v-show="expand2"
          height="90%"
          width="100%"
          class="mx-auto"
          style="position: absolute; top: 5%; left: 98%; border-radius: 2em; border-top-left-radius: 0; border-bottom-left-radius: 0;"
        ></v-card>
      </v-expand-x-transition>
      </v-card>
      
    </v-container>
  </div>
</template>

<script>
export default {
    data: ()=> ({
        expand: false,
        expand2: false
    })
}
</script>

<style>
h1 {
  text-align: center;
}

.midImg {
  padding-left: 5%;
}
</style>

<style lang="scss">
.rounded {
  border-radius: 50;
}
@font-face {
  font-family: "Product Sans";
  font-style: normal;
  font-weight: 700;
  src: local("Open Sans"), local("OpenSans"),
    url(https://fonts.gstatic.com/s/productsans/v5/HYvgU2fE2nRJvZ5JFAumwegdm0LZdjqr5-oayXSOefg.woff2)
      format("woff2");
}

* {
  text-transform: none !important;
  letter-spacing: 0.04em;
  font-family: Product Sans;
}
</style>