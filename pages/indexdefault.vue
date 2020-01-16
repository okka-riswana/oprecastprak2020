<template>
  <v-layout
    wrap
  >
    <v-flex
      xs12
      sm12
      md12
    >
      <banner />
      <v-card>
        <v-card-title class="headline">
          What?
        </v-card-title>
        <div class="pa-5">
          <v-row
            class="mb-6"
          >
            <v-col
              md="6"
              sm="6"
            >
              <ul class="body-1">
                <li>As the facilitator, share your knowledge.</li>
                <li>Delivering the subject to students.</li>
                <li>Create, conduct, and examine assignments.</li>
                <li>Responsible for laboratory maintenance.</li>
              </ul>
            </v-col>
            <v-col
              md="6"
              sm="6"
            >
              <ul class="body-1">
                <li>As the facilitator, share your knowledge.</li>
                <li>Delivering the subject to students.</li>
                <li>Create, conduct, and examine assignments.</li>
                <li>Responsible for laboratory maintenance.</li>
              </ul>
            </v-col>
          </v-row>
        </div>
        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/inspire"
          >
            Register Now
          </v-btn>
        </v-card-actions>
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
