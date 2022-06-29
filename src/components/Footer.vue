<template>
  <div>
      <footer dark padless>
        <v-card flat tile width="100%" class="primary white--text text-center">
          <v-row justify="center" no-gutters>
            <v-btn
              v-for="link in links"
              :key="link"
              color="white"
              text
              rounded
              class="my-2"
            >
              {{ link }}
            </v-btn>
          </v-row>

          <!-- bottom item -->
          <v-card-text>
            <h2 class="pb-2 white--text">میتوانید مارا دنبال کنید در</h2>
            <a target="_blank" href="#">
              <v-btn class="mx-4 white--text" icon>
                <v-icon size="24px">mdi-github</v-icon>
              </v-btn>
            </a>
            <a target="_blank" href="#">
              <v-btn class="mx-4 white--text" icon>
                <v-icon size="24px">mdi-gitlab</v-icon>
              </v-btn>
            </a>
            <a target="_blank" href="#">
              <v-btn class="mx-4 white--text" icon>
                <v-icon size="24px">mdi-facebook</v-icon>
              </v-btn>
            </a>
            <a target="_blank" href="#">
              <v-btn class="mx-4 white--text" icon>
                <v-icon size="24px">mdi-twitter</v-icon>
              </v-btn>
            </a>
            <a target="_blank" href="#">
              <v-btn class="mx-4 white--text" icon>
                <v-icon size="24px">mdi-google</v-icon>
              </v-btn>
            </a>
            <a target="_blank" href="#">
              <v-btn class="mx-4 white--text" icon>
                <v-icon size="24px">mdi-linkedin</v-icon>
              </v-btn>
            </a>
            <a target="_blank" href="#">
              <v-btn class="mx-4 white--text" icon>
                <v-icon size="24px">mdi-instagram</v-icon>
              </v-btn>
            </a>
          </v-card-text>
        </v-card>
      </footer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      links: [
        'Home',
        'About Us',
        'Team',
        'Services',
        'Blog',
        'Contact Us',
      ],
    };
  },
};
</script>

<style scoped>
</style>