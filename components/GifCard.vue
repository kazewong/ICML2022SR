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
    <v-row>
      <v-col cols="12" sm="8">
        <video class="illustration" autoplay>
          <source :src="image" type="video/mp4">

        </video>
      </v-col>
      <v-col cols="0" sm="4">
        <v-card-text>
          <p>
            {{ body }}
          </p>
        </v-card-text>
      </v-col>
    </v-row>
  </v-card>
</template>

<style>

.illustration {
  height: 100%;
  width: 100%;
  max-width: 600px;
  padding-left: 10px;
}
</style>
