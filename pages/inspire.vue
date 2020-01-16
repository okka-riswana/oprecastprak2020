<template>
  <v-layout>
    <v-flex>
      <banner />
      <v-card>
        <v-card-title>
          Requirements
        </v-card-title>
        <v-card-text>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </v-card-text>
      </v-card>
      <div class="my-3">
        <h1>Timeline</h1>
        <timeline />
      </div>
    </v-flex>
  </v-layout>
</template>
<script>
import Banner from '~/components/Banner.vue'
import Timeline from '~/components/Timeline.vue'

export default {
  components: {
    Timeline,
    Banner
  }
}
</script>
