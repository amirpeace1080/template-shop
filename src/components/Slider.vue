<template>
  <v-carousel height="500" hide-delimiter-background show-arrows-on-hover>
    <v-carousel-item>
      <v-sheet color="blue lighten-1" fill-height height="100%">
        <v-row class="fill-height" align="center" justify="center">
          <div class="text-h2">Slide One</div>
        </v-row>
      </v-sheet>
    </v-carousel-item>
    <v-carousel-item>
      <v-sheet color="warning" height="100%">
        <v-row class="fill-height" align="center" justify="center">
          <div class="text-h2">Slide Two</div>
        </v-row>
      </v-sheet>
    </v-carousel-item>
    <v-carousel-item>
      <v-sheet color="info" height="100%">
        <v-row class="fill-height" align="center" justify="center">
          <div class="text-h2">Slide Three</div>
        </v-row>
      </v-sheet>
    </v-carousel-item>
    <v-carousel-item>
      <v-sheet color="primary" height="100%">
        <v-row class="fill-height" align="center" justify="center">
          <div class="text-h2">Slide Four</div>
        </v-row>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
</template>

<script>
export default {
  data() {
    return {
      //
    }
  },
};
</script>