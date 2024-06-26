<template>
  <v-divider class="" color="red-darken-4"></v-divider>
  <v-sheet id="samples" class="text-center py-16">
    <div class="text-h3 text-grey-lighten-3 font-weight-regular">
      Drum Samples
    </div>

    <div class="text-body-1 text-medium-emphasis my-5">
      An assortment of free one-shot drum samples I've made; all released under CC0 1.0 for free use.
    </div>

    <v-container>
      <v-row>
        <v-col v-for="drum in samples" :key="drum.title" class="ga-5 pa-5" cols="12" md="4">
          <div class="mt-1">
            <v-icon :icon="drum.icon" color="red-lighten-1" size="x-large" variant="text"></v-icon>
          </div>

          <div>
            <div class="text-overline font-weight-light">
              {{ drum.title }}
            </div>

            <div class="">
              <span v-html="drum.audio"></span>
            </div>
          </div>

        </v-col>
      </v-row>
    </v-container>
    <v-btn :block="$vuetify.display.mdAndDown" size="large" elevation="3" color="red-darken-3" height="55"
      href="#samples" text="Download" />
  </v-sheet>
  <v-divider color="red-darken-4"></v-divider>
</template>

<style>
audio {
  /*filter: sepia(20%) saturate(70%) grayscale(1) contrast(99%) invert(12%); */
  width: 200px;
  height: 50px;

  background-color: #263238;
}
</style>
  
<script setup>
const samples = [
  {
    icon: 'mdi-nuke',
    title: 'Tactical Snare Nuke',
    audio:
      '<audio controls>  <source src="/assets/samples/1.mp3" type="audio/mpeg">Your browser does not support the audio element. </audio> ',
  },
  {
    icon: 'mdi-controller',
    title: 'Kwick Scope',
    audio:
      '<audio controls>  <source src="/assets/samples/1.mp3" type="audio/mpeg">Your browser does not support the audio element. </audio> ',
  },
  {
    icon: 'mdi-bomb',
    title: 'Knick Cannon',
    audio:
      '<audio controls>  <source src="/assets/samples/1.mp3" type="audio/mpeg">Your browser does not support the audio element. </audio> ',
  },
  {
    icon: 'mdi-alert',
    title: 'War Room Snare',
    audio:
      '<audio controls>  <source src="/assets/samples/1.mp3" type="audio/mpeg">Your browser does not support the audio element. </audio> ',
  },
  {
    icon: 'mdi-knife-military',
    title: 'Combat Tom',
    audio:
      '<audio controls>  <source src="/assets/samples/1.mp3" type="audio/mpeg">Your browser does not support the audio element. </audio> ',
  },
  {
    icon: 'mdi-submarine',
    title: 'Floor Tom Torpedo',
    audio:
      '<audio controls>  <source src="/assets/samples/1.mp3" type="audio/mpeg">Your browser does not support the audio element. </audio> ',
  },
]
</script>
