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
      class="mt-5 mb-12"
    >
      <v-expansion-panels>
        <v-expansion-panel
          v-for="faq in faqs"
        >
          <v-expansion-panel-header>
            <b>{{ faq.q }}</b>
          </v-expansion-panel-header>
          <v-expansion-panel-content>
            <b>Answer : </b>{{ faq.a }}
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-flex>
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

export default {
  components: {
    Banner
  },
  data: () => ({
    cp1: 'Marcell Antonius (Line ID : marcell_antonius14)',
    cp2: 'Faradilla Azranur (Line ID : fardil7)',
    faqs: [
      {
        q: 'Bahasa apa yang harus digunakan untuk Cover Letter, CV, dan Self-Introduction Video?',
        a: 'Bahasa yang digunakan bebas, Bahasa Indonesia atau Bahasa Inggris tidak masalah.'
      },
      {
        q: 'Bagaimana isi Self-Introduction Video?',
        a: 'Harus memperlihatkan diri, perkenalkan diri, alasan mau menjadi asprak, buat sekreatif mungkin. Pastikan account Instagram tidak di-private ya.'
      },
      {
        q: 'Isi Cover Letter?',
        a: 'Sesuai dengan isi cover letter formal pada umumnya, seperti saat akan melamar suatu pekerjaan.'
      },
      {
        q: 'Mata kuliah apa saja yang harus minimal B?',
        a: 'Tidak ada ketentuan mata kuliah apa saja, yang penting IPK diatas 3.00. Persyaratan nilai mata kuliah tertentu minimal B hanya digunakan ketika memilih mata kuliah apa yang diajarkan nanti.'
      },
      {
        q: 'Test coding? Apa yang harus dipersiapkan?',
        a: 'Tidak rumit, test ini untuk melihat sejauh mana kalian menyelesaikan suatu permasalahan dasar dengan logika sederhana. Untuk apa yang harus dipersiapkan, bagaimana prosesnya akan diinformasikan kepada pendaftar.'
      }
    ]
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
