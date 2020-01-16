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
      <v-row
        align="center"
        justify="center"
      >
        <v-col cols="6">
          <h1
            class="font-weight-thin mb-4 ml-7 absolute"
            :class="{'display-1': $vuetify.breakpoint.smAndDown, 'display-3': $vuetify.breakpoint.mdAndUp}"
          >
            OPEN RECRUITMENT
          </h1>
          <h4
            class="mb-5 ml-7"
            :class="{'body-1': $vuetify.breakpoint.smAndDown, 'display-1': $vuetify.breakpoint.mdAndUp}"
          >
            Laboratory Assistant 2020
          </h4>
          <v-btn
            class="ml-7"
            depressed
            color="primary"
            to="/requirements"
            router
            exact
          >
            Register Now
          </v-btn>
        </v-col>
        <v-col cols="6">
          <v-img
            src="/bg_asprak.svg"
            max-width="100%"
          >
          </v-img>
        </v-col>
      </v-row>
    </v-flex>
    <div class="line">
    </div>
    <v-flex
      xs12
      sm8
      md10
      class="mt-5"
      align-self-center="true"
    >
      <v-row
        justify="center"
      >
        <h1 class="display-1">WHAT?</h1>
      </v-row>
      <v-row
        align="center"
        justify="center"
        class="pl-12 pr-12 mt-6"
      >
        <v-flex xs12 sm6 md3 pr-4 pt-4>
          <v-card shaped>
            <v-card-title class="body-1" style="background: rgba(253, 210, 49, 0.2);">
              As the facilitator, share your knowledge.
            </v-card-title>
          </v-card>
        </v-flex>
        <v-flex xs12 sm6 md3 pr-4 pt-4>
          <v-card shaped>
            <v-card-title class="body-1" style="background: rgba(155, 81, 224, 0.2);">
              Delivering the subject to students.
            </v-card-title>
          </v-card>
        </v-flex>
        <v-flex xs12 sm6 md3 pr-4 pt-4>
          <v-card shaped>
            <v-card-title class="body-1" style="background: rgba(80, 211, 141, 0.2);">
              Create, conduct, and examine assignments.
            </v-card-title>
          </v-card>
        </v-flex>
        <v-flex xs12 sm6 md3 pr-4 pt-4>
          <v-card shaped>
            <v-card-title class="body-1" style="background: rgba(253, 210, 49, 0.2);">
              Responsible for laboratory maintenance.
            </v-card-title>
          </v-card>
        </v-flex>
      </v-row>
    </v-flex>
    <v-flex
      xs12
      sm8
      md10
      class="mt-12"
      align-self-center="true"
    >
      <v-row
        justify="center"
      >
        <h1 class="display-1">WHY?</h1>
      </v-row>
      <v-row
        align="center"
        justify="center"
        class="pl-12 pr-12 mt-6"
      >
        <v-flex xs12 sm6 md3 pr-4 pt-4>
          <v-card shaped>
            <v-card-title class="body-1" style="background: rgba(253, 210, 49, 0.2);">
              Gain valuable experience.
            </v-card-title>
          </v-card>
        </v-flex>
        <v-flex xs12 sm6 md3 pr-4 pt-4>
          <v-card shaped>
            <v-card-title class="body-1" style="background: rgba(155, 81, 224, 0.2);">
              Develop and refine your skills.
            </v-card-title>
          </v-card>
        </v-flex>
        <v-flex xs12 sm6 md3 pr-4 pt-4>
          <v-card shaped>
            <v-card-title class="body-1" style="background: rgba(80, 211, 141, 0.2);">
              Gain confidence.
            </v-card-title>
          </v-card>
        </v-flex>
        <v-flex xs12 sm6 md3 pr-4 pt-4>
          <v-card shaped>
            <v-card-title class="body-1" style="background: rgba(253, 210, 49, 0.2);">
              Other good benefits.
            </v-card-title>
          </v-card>
        </v-flex>
      </v-row>
    </v-flex>
    <div class="line">
    </div>
    <v-flex
      xs12
      sm8
      md10
      class="mt-5"
    >
      <v-row
        justify="center"
      >
        <h1 class="display-1 mb-6">COURSE</h1>
      </v-row>
      <v-flex class="pl-12 pr-12 text-center body-1">
        <p>Data Structure, Architecture & Organization of Computer, Database System I, Computer Networks, Digital Image Processing, Artificial Intelligence, Information System Multimedia, Analytics Algorithm, Distributed Database.</p>
        <p>Algorithm & Programming, Numerical Method, Cryptography, Robotic, Object Oriented Programming I, Software Engineering, Web Programming, Database System II.</p>
      </v-flex>
    </v-flex>
    <div class="line">
    </div>
    <v-flex
      xs12
      sm8
      md10
      class="mt-5"
    >
      <v-row
        justify="center"
      >
        <h1 class="display-1 mb-6">OUR FAMILY</h1>
      </v-row>
      <v-flex>
        <Gallery />
      </v-flex>
    </v-flex>
    <v-flex
      xs12
      sm12
      md12
      class="text-center"
    >
      <v-btn
        class="ml-7"
        depressed
        color="primary"
        to="/requirements"
        router
        exact
      >
        Register Now
      </v-btn>
    </v-flex>
    <div class="line">
    </div>
  </v-layout>
</template>

<script>
import Gallery from '~/components/Gallery.vue'

export default {
  components: {
    Gallery
  }
}
</script>
<style>
.line{
  background-color: rgba(99, 163, 227, 0.6);
  height: 3px;
  width: 80%;
  margin-top: 40px;
  margin-bottom: 10px;
}
</style>
