<template>
  <v-layout
    column
    justify-center
    align-center
  >
    <v-flex
      xs12
      sm8
      md6
    >
      <banner />
      <v-card>
        <v-card-title class="headline">
          Welcome All
        </v-card-title>
        <v-card-text>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
        </v-card-text>
        <!-- <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/inspire"
          >
            Next
          </v-btn>
        </v-card-actions> -->
      </v-card>
      <v-card class="my-3">
        <v-card-title class="headline">
          What?
        </v-card-title>
        <v-card-text>
          <p>teakrael</p>
        </v-card-text>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
import Banner from '~/components/Banner.vue'

export default {
  components: {
    Banner
  }
}
</script>
