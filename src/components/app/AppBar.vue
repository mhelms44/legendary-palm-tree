<template>
    <v-app-bar :elevation="5" class="">
      <template #title>
        <div class="d-inline-flex align-center text-h5 font-weight-bold my-5 text-primary">
  
          <span class="text-grey-lighten-3">Weaponized Audio</span>
        </div>
      </template>
  
      <template v-if="$vuetify.display.mdAndUp" #append>
        <div class="hidden-sm-and-down">
          <v-btn
            v-for="item in menu"
            :key="item"
            class="text-body-2 text-grey-lighten-3"
            :href="`#${item.toLowerCase()}`"
            variant="text"
          >
            {{ item }}
          </v-btn>
        </div>
      </template>
    </v-app-bar>
  </template>
  
  <script setup>
    const menu = [
      'Discography',
      'Samples',
      'Tools',
    ]
  </script>
  