<template>
  <v-layout
    wrap
    align-center
    justify-center
  >
    <v-flex
      xs12
      sm12
      md12
    >
      <Banner title="REQUIREMENTS" subtitle="Timeline Recruitment" />
    </v-flex>
    <div class="line2">
    </div>
    <v-flex
      xs10
      sm10
      md10
    >
      <v-row
        class="mt-5"
        justify="center"
      >
        <h1 class="display-1 mb-6">HELLO!</h1>
      </v-row>
      <v-row
        justify="center"
        class="text-center"
      >
        <p class="body-1">Want to take part in 2020 Lab Assistant selection? Well there are some things that you must prepare.<br> See the info below for the selection flow.</p>
      </v-row>
    </v-flex>
    <div class="line2">
    </div>
    <v-flex
      xs10
      sm10
      md10
    >
      <v-row
        class="mt-5"
        justify="center"
      >
        <h1 class="display-1 mb-6">TIMELINE</h1>
      </v-row>
      <div class="my-3">
        <timeline />
      </div>
      <v-row
        class="mt-5"
        justify="center"
      >
        <v-btn
          class="ml-7 white--text"
          depressed
          color="red darken-1"
          href="https://docs.google.com/forms/d/e/1FAIpQLSd3wpdY3_r5UnVbDF5uUmuChMUza4HziizyiuGdmF79Ngx-AQ/viewform"
          target="_blank"
        >
          Register Now
        </v-btn>
      </v-row>
    </v-flex>
    <v-flex
      xs10
      sm10
      md10
      class="mt-12"
    >
      <h1 class="title">Further Questions?</h1>
      <p class="body-1">Drop your question to <b>{{ cp1 }}</b> or <b>{{ cp2 }}</b></p>
      <v-row
        justify="center"
      >
        <v-btn
          class="font-weight-bold"
          color="primary"
          text
          to="/faq"
          router
          exact
        >
          Frequently Asked Questions
        </v-btn>
      </v-row>
    </v-flex>
    <div class="line2">
    </div>
  </v-layout>
</template>

<script>
import Banner from '~/components/Banner.vue'
import Timeline from '~/components/Timeline.vue'

export default {
  components: {
    Timeline,
    Banner
  },
  data: () => ({
    cp1: 'Marcell Antonius (Line ID : marcell_antonius14)',
    cp2: 'Faradilla Azranur (Line ID : fardil7)'
  })
}
</script>

<style>
.line2{
  background-color: rgba(215, 79, 46, 1);
  height: 3px;
  width: 80%;
  margin-top: 40px;
  margin-bottom: 10px;
}
</style>
