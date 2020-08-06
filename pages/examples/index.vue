<template>
  <div class="examples">
       <nuxt-link to="/"><v-btn text color="blue">Menu</v-btn></nuxt-link>
      <h1>Examples</h1>
      <v-container v-for="example in examples" v-bind:key="example" style="display: inline-flex">
          <v-card width="20%" style="border-radius: 2.5em" class="ms-10" :href="`${example.link}`" >
        <v-container>
          <v-btn fab color="blue" style="position: absolute; z-index: 5; border-radius: 1.4em; height: 63px; left: -2em; top: -1em;" :href="`${example.github}`"> 
              <v-icon x-large>mdi-github</v-icon>
              </v-btn>
          <v-img
            max-height="100%"
            max-width="100%"
            fit
            :src="`${example.img}`"
            style="border-radius: 1.5em;"
          ></v-img>
          <div>
            <v-card-title>{{example.title}}</v-card-title>
            <v-card-subtitle>{{example.subtitle}}</v-card-subtitle>
          </div>
        </v-container>
      </v-card>
      </v-container>
  </div>
</template>

<script>
export default {
    data: () => ({
        examples: [
            {title: 'UI Coursework 3', subtitle: 'Firebase Calendar', github: 'https://github.com/Dhrushil', link:'https://uicw3-final.web.app/', img: '/UICW3.jpg'},
            {title: 'Travel Co', subtitle: 'Personalised trip manager', github: 'https://github.com/Dhrushil', link:'https://travel-co-841db.web.app/', img: '/travelco.jpg'},
        ]
    })
}
</script>

<style>
h1 {
    text-align: center;
}
</style>