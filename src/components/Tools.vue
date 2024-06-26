<template>
  <v-sheet id="tools" class="py-16 text-center" color="#121212">
    <div class="text-h3 text-grey-lighten-3 font-weight-regular">
      Tools
    </div>

    <div class="text-body-1 text-medium-emphasis ma-10 px-16">
      <span class="px-16">Some scripts/utilities I've made that might be useful. These are all generally Windows/Reaper
        specific.
        Let me know if you run into any problems using them and feel free to modify them as needed.
      </span>
    </div>

    <v-container>
      <v-row>
        <v-col v-for="item in tools" :key="item.title" class="d-flex flex-column align-center" cols="12" md="4">
          <v-btn :icon="item.icon" color="light-blue-accent-4" size="x-large" variant="text" :href="item.url">
          </v-btn>
          <div class="text-overline font-weight-light mt-2"> {{ item.title }}</div>

          <div class="text-body-2 mt-2 text-medium-emphasis w-75">
            {{ item.description }}
          </div>
        </v-col>
      </v-row>
    </v-container>
  </v-sheet>
</template>

<script setup>
const tools = [
  {
    icon: 'mdi-content-save',
    url: 'https://github.com/mhelms44/reabak',
    title: 'ReaBak',
    description:
      'Powershell scripts to automate backing up Reaper projects and optionally compress them with LZX.',
  },
  {
    icon: 'mdi-content-copy',
    url: 'https://github.com/mhelms44/reabak',
    title: 'Steven Slate Drums Reaper Template',
    description:
      'Setting up multi-track routing in Reaper with SSD or any other sampler is not too painful, but this helps get you rolling quicker.',
  },
  {
    icon: 'mdi-book-cog',
    url: 'https://github.com/mhelms44/reabak',
    title: 'Reaper Custom Actions',
    description:
      'Custom actions/macros for Reaper to speedup certain workflows.',
  },
]
</script>