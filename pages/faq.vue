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
      <Banner title="FAQ" subtitle="Frequently Asked Questions" />
    </v-flex>
    <div class="line2">
    </div>
    <v-flex
      xs10
      sm10
      md10
      class="mt-5"
    >
      <Faq />
    </v-flex>
    <div class="line2">
    </div>
    <v-flex
      xs10
      sm10
      md10
      class="mt-12"
    >
      <h1 class="title">Further Questions?</h1>
      <p class="body-1">Drop your question to <b>{{ cp1 }}</b> or <b>{{ cp2 }}</b></p>
    </v-flex>
    <div class="line2">
    </div>
  </v-layout>
</template>

<script>
import Banner from '~/components/Banner.vue'
import Faq from '~/components/Faq.vue'

export default {
  components: {
    Banner,
    Faq
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
