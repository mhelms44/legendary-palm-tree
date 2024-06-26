<template>

  <v-card id="home" class="d-flex justify-center align-center text-center flex-column bg-blue-grey-darken-4"
    min-height="600">
    
    <div class="text-h2 font-weight-regular mb-5 text-grey-lighten-5">
      Forging sounds that shred
    </div>
    
    <div class="text-h6 font-weight-light mb-5 px-5 text-white" style="max-width: 600px;">
      Hey there, I'm Michael! I work with artists to get the best out
      of their music. Let's work together to take your project to the next level. Click the button below to get started!
    </div>

    <div class="d-flex ga-5 flex-1-1-auto flex-wrap justify-center px-4">

      <v-btn :block="$vuetify.display.mdAndDown" size="large" elevation="6" color="red-darken-3" flat height="55"
        href="https://forms.gle/FxMbdDwwbSZWcS5y5" text="Google contact form" />
    </div>

  </v-card>

  <v-divider thickness="2" color="blue"></v-divider>
</template>