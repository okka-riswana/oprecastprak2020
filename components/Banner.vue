<template>
  <v-parallax
    src="/bg_asprak1.jpg"
    height="400"
  >
    <v-row
      align="center"
      justify="center"
    >
      <v-col class="text-center" cols="12">
        <h1
          class="font-weight-bold mb-4"
          :class="{'display-1': $vuetify.breakpoint.smAndDown, 'display-3': $vuetify.breakpoint.mdAndUp}"
        >
          {{ title }}
        </h1>
        <hr class="my-2">
        <h4
          class="display-1"
          :class="{'body-1': $vuetify.breakpoint.smAndDown, 'display-1': $vuetify.breakpoint.mdAndUp}"
        >
          {{ subtitle }}
        </h4>
      </v-col>
    </v-row>
  </v-parallax>
</template>

<script>
export default {
  props: ['title', 'subtitle']
}
</script>
