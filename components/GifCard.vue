<script>
export default {
  props: {
    title: {
      type: String,
      default: 'Fill me in'
    },
    body: {
      type: String,
      default: 'Fill me in'
    },
    image: {
      type: String,
      default: 'Fill me in'
    }
  }
}
</script>

<template>
  <v-card>
    <v-card-title class="headline">
      {{ title }}
    </v-card-title>
    <v-card-text>
      <p>
        {{ body }}
      </p>
    </v-card-text>
    <img
      class="vuetify-logo"
      alt="Vuetify Logo"
      :src="image"
    >
  </v-card>
</template>

<style>

</style>
