<template>
    <v-sheet
      id="discography"
      class="text-center py-16"
      color="background"
      min-height="800"
    >
      <div class="text-h3 text-grey-lighten-3 font-weight-regular">
        Discography
      </div>
  
      <div class="text-body-1 text-medium-emphasis mt-5">
      </div>
  
      <v-container class="w-75 w-xl-50">
        <v-row>
          <v-col
            v-for="release in releases"
            :key="release.title"
            class="pa-5"
            cols="12"
            md="4"
          >
            <v-card
              class="bg-black rounded-t-xl pb-5"
              :href="release.url"
              elevation="16"
            >
              <v-img
              :src="release.image" aspect-ratio="1/1" cover
              class="w-100 rounded-t-xl"  
              />
  
              <div class="mt-2 text-body-1">
                {{ release.name }}
              </div>
  
              <div class="mt-1 text-grey-lighten-2 font-italic text-body-1">
                {{ release.title }}
              </div>

              <div class="mt-1 text-caption text-center text-grey-lighten-1 px-5">
                {{ release.credits }}
              </div>

            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-sheet>
  </template>
  
  <script setup>
    const releases = [
      {
        image: './assets/coverart/rlam.jpg',
        name: 'Alpha Andromeda',
        title: 'RLAM',
        credits: 'Producer, Engineer, Editing, Mixing, Mastering',
        url:
          'https://alphaandromeda.bandcamp.com/track/rlam',
      },
      {
        image: './assets/coverart/stts.jpg',
        name: 'Alpha Andromeda',
        title: 'Submit To the Swarm',
        credits: 'Producer, Engineer, Editing, Mixing, Mastering',
        url:
          'https://alphaandromeda.bandcamp.com/track/submit-to-the-swarm',
      },
      {
        image: './assets/coverart/granny.jpg',
        name: 'Alpha Andromeda',
        title: 'Ominous Mechanobiology',
        credits: 'Producer, Engineer, Editing, Mixing, Mastering',
        url:
          'https://alphaandromeda.bandcamp.com/track/ominous-mechanobiology',
      },
      {
        image: './assets/coverart/rope.jpg',
        name: 'Alpha Andromeda',
        title: 'A Good Rope And A Strong Branch',
        credits: 'Producer, Engineer, Editing, Mixing, Mastering',
        url:
          'https://alphaandromeda.bandcamp.com/track/a-good-rope-and-a-strong-branch',
      },
      {
        image: './assets/coverart/junko.jpg',
        name: 'Alpha Andromeda',
        title: 'Junko',
        credits: 'Producer, Engineer, Editing, Mixing, Mastering',
        url:
          'https://alphaandromeda.bandcamp.com/track/junko',
      },
      {
        image: './assets/coverart/void.jpg',
        name: 'Alpha Andromeda',
        title: 'Gaze Into The Void',
        credits: 'Producer, Engineer, Editing, Mixing, Mastering',
        url:
          'https://alphaandromeda.bandcamp.com/track/gaze-into-the-void',
      },
      {
        image: './assets/coverart/bc-home.jpg',
        name: 'Busted Chops',
        title: 'Home',
        credits: 'Mixing, Mastering',
        url:
          'https://bustedchops.bandcamp.com/album/home',
      },
      {
        image: './assets/coverart/apeirogon.jpg',
        name: 'Polygons',
        title: 'Apeirogon',
        credits: 'Producer, Engineer, Editing, Mixing, Mastering',
        url:
          'https://polygonsnc.bandcamp.com/album/apeirogon',
      },
      {
        image: './assets/coverart/bc-gnarly.jpg',
        name: 'Busted Chops',
        title: 'Illumignarly',
        credits: 'Mixing, Mastering',
        url:
          'https://bustedchops.bandcamp.com/album/illumignarly',
      },
      {
        image: './assets/coverart/asylum.jpg',
        name: 'Asylum',
        title: 'By My Side',
        credits: 'Tracks 1-4 Engineer, Editing, Mixing, Mastering',
        url:
          'https://asylumnc.bandcamp.com/album/by-my-side',
      },
      {
        image: './assets/coverart/rifts.jpg',
        name: 'Polygons',
        title: 'Rifts',
        credits: 'Producer, Engineer, Editing, Mixing, Mastering',
        url:
          'https://polygonsnc.bandcamp.com/album/rifts',
      },
      {
        image: './assets/coverart/nw-self.jpg',
        name: 'Naomi Wise',
        title: 'Naomi Wise EP',
        credits: 'Engineer, Editing, Mixing, Mastering',
        url:
          'https://naomiwise.bandcamp.com/album/naomi-wise-ep-2',
      },
      {
        image: './assets/coverart/bc-ohman.jpg',
        name: 'Busted Chops',
        title: 'Oh, man',
        credits: 'Mixing, Mastering',
        url:
          'https://polygonsnc.bandcamp.com/album/do-u-evn-lift-bro',
      },
      {
        image: './assets/coverart/lift.jpg',
        name: 'Polygons',
        title: 'do u evn lift bro -_____-',
        credits: 'Producer, Engineer, Editing, Mixing, Mastering',
        url:
          'https://polygonsnc.bandcamp.com/album/do-u-evn-lift-bro',
      },


    ]
  </script>
  
  