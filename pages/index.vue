<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <v-card class="logo py-4 d-flex justify-center">
        <PySRLogo />
      </v-card>
      <v-card>
        <GifCard
          title="TL;DR"
          body="This is a simple Vue.js app that uses Vuetify to build a simple Gif Card."
          image="/GW_population.mp4"
        />

        <GifCard
          title="Premise in gravitational wave"
          body="This is a simple Vue.js app that uses Vuetify to build a simple Gif Card."
          image="/PhenomenologicalModelling.mp4"
        />
        <v-card-title class="headline">
          Symoblic regression
        </v-card-title>
        <v-card-text>
          <p>
            Insert example for interactive symbolic regression
          </p>
        </v-card-text>
        <v-card-title class="headline">
          Test
        </v-card-title>
        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/inspire"
          >
            Continue
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>
