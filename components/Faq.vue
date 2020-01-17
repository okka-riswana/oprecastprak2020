<template>
  <v-expansion-panels>
    <v-expansion-panel
      v-for="faq in faqs"
    >
      <v-expansion-panel-header class="body-1 font-weight-bold">
        {{ faq.q }}
      </v-expansion-panel-header>
      <v-expansion-panel-content class="body-1">
        <b>Answer : </b>{{ faq.a }}
      </v-expansion-panel-content>
    </v-expansion-panel>
  </v-expansion-panels>
</template>

<script>
export default {
  data: () => ({
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
      },
      {
        q: 'Upload jawaban online assessment kemana?',
        a: 'Upload di web ini, nanti akan muncul button upload di halaman timeline recruitment pada tanggal 2 Februari 2020 pukul 13.00 WIB.'
      }
    ]
  })
}
</script>
