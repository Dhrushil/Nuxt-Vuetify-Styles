<template>
  <v-layout>
    <v-flex class="text-center">
      <img
        src="/v.png"
        alt="Vuetify.js"
        class="mb-5"
      >
      <blockquote class="blockquote">
        &#8220;First, solve the problem. Then, write the code.&#8221;
        <footer>
          <small>
            <em>&mdash;John Johnson</em>
          </small>
        </footer>
      </blockquote>
    </v-flex>

    <v-btn text x-small style="top: 0.5em; border-radius: 1em" @click="expand = !expand">reply</v-btn>
                          <v-expand-transition>
        <v-card
          v-show="expand"
          height="100"
          width="100"
          class="mx-auto"
        ></v-card>
      </v-expand-transition>
  </v-layout>
</template>

<script>
export default {
  data: ()=> ({
    expand: false
  })
}
</script>