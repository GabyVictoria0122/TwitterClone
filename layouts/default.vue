<template>
  <v-app id="inspire">
    <v-main class="grey lighten-3">
      <v-container>
        <v-row>
          <v-col
            cols="12"
            sm="2"
            class="mt-0 pt-0"
          >
            <v-sheet
              rounded="lg"
              min-height="268"
            >
              <Menu/>
            </v-sheet>
          </v-col>

          <v-col
            cols="12"
            sm="8"
            class="mt-0 pt-0"
          >
            <v-sheet
              min-height="70vh"
              rounded="lg"
            >
            <Nuxt/>
          </v-sheet>
          </v-col>

          <v-col
            cols="12"
            sm="2"
            class="mt-0 pt-0"
          >
           <v-sheet
              rounded="lg"
              min-height="268"
            >
              <SearchTwitter/>
            </v-sheet>
            <v-sheet
              rounded="lg"
              min-height="268"
            >
              <WhatHappening/>
            </v-sheet>
             <v-sheet
              rounded="lg"
              min-height="268"
            >
              <WhoFollow/>
            </v-sheet>
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import Menu from '../components/Menu.vue'
import SearchTwitter from '../components/SearchTwitter.vue'
import WhoFollow from '../components/WhoFollow.vue'
import WhatHappening from '../components/WhatHappening.vue'
export default {
  name: 'DefaultLayout',
  components: {
    Menu,
    SearchTwitter,
    WhoFollow,
    WhatHappening
  },
  data () {
    return {
      // links: [
      //   'Página Inicial'
      // ]
    }
  }
}
</script>
