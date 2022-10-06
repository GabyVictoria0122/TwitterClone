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
              <!--  -->
                            <!-- <h1>Menu</h1> -->

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
              <!--  -->
              <h1>Buscar no Twitter </h1>

            </v-sheet>
            <v-sheet
              rounded="lg"
              min-height="268"
            >
              <!--  -->
              <h1>O que está acontecendo</h1>

            </v-sheet>
             <v-sheet
              rounded="lg"
              min-height="268"
            >
              <!--  -->
              <h1>Quem seguir</h1>

            </v-sheet>
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {
      // links: [
      //   'Página Inicial'
      // ]
    }
  }
}
</script>
