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
  },
  data () {
    return {
      show: false
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
        <button @click="show = !show">
          Toggle
        </button>
        <v-slide-x-transition>
          <v-card-text v-show="show">
            <p>
              {{ body }}
            </p>
          </v-card-text>
        </v-slide-x-transition>
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

.slide-fade-enter-active {
  transition: all 0.3s ease-out;
}

.slide-fade-leave-active {
  transition: all 0.8s cubic-bezier(1, 0.5, 0.8, 1);
}

.slide-fade-enter-from,
.slide-fade-leave-to {
  transform: translateX(20px);
  opacity: 0;
}
</style>
