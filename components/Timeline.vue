<template>
  <v-timeline align-top :dense="$vuetify.breakpoint.smAndDown">
    <v-timeline-item
      v-for="(item, i) in items"
      :key="i"
      :color="item.color"
      :icon="item.icon"
      fill-dot
    >
      <span slot="opposite" class="body-1 font-weight-bold" :class="item.color + '--text'">{{ item.date }}</span>
      <v-card
        :color="item.color"
        dark
      >
        <v-card-title class="title">{{ item.title }}</v-card-title>
        <v-card-text class="white body-1 text--primary">
          <span>{{ item.desc_det }}</span>
          <ul class="pa-5">
            <li
              v-for="desc in item.descs"
            >
              {{ desc }}
            </li>
            <ul>
              <li
                v-for="kriteria in item.kriteria_video"
              >
                {{ kriteria }}
              </li>
            </ul>
          </ul>
          <v-btn
            v-if="typeof item.link_upload_jawaban != 'undefined'"
            outlined
            :color="item.color"
            :href="item.link_upload_jawaban"
            target="_blank"
            hidden
          >
            Upload Answer
          </v-btn>
          <span
            class="body-1 font-weight-bold"
            :class="item.color + '--text'"
            v-if="typeof item.date != 'undefined' && $vuetify.breakpoint.smAndDown"
          >
            {{ item.date }}
          </span>
        </v-card-text>
      </v-card>
    </v-timeline-item>
  </v-timeline>
</template>
<script>
export default {
  data: () => ({
    items: [
      {
        color: 'red lighten-2',
        icon: 'mdi-star',
        title: 'Make sure you are fit the requirements.',
        descs: [
          'Anggota Penuh Himatif FMIPA Unpad and currently in third year (2017) or second year (2018).',
          'Minimum GPA 3.00.',
          'Have minimum grade B for the subject you wanted.'
        ]
      },
      {
        color: 'purple',
        icon: 'mdi-book-variant',
        title: 'Registration & Pre-screening Assessment.',
        date: '17 January 2020 - 31 January 2020',
        descs: [
          'Register yourself, fill the form.',
          'Upload the requirement files (CV, Cover Letter) in pdf files.',
          'Upload your Academic Transcript from students.unpad.ac.id',
          'Submit Instagram links for short introduction video. The Rules of Video :'
        ],
        kriteria_video: [
          'Make sure your own face is shown',
          'Introduce yourself',
          'The reason why you want to be part of us',
          'Make it as creative as possible',
          'Use hashtag #oprectasprak2020',
          'Make sure your instagram account is not private'
        ]
      },
      {
        color: 'green',
        icon: 'mdi-laptop',
        title: 'Online Assessment.',
        date: '2 February 2020 start at 1 PM WIB',
        descs: [
          'A test for your basic skills.',
          'You will be given a chance to answer some questions in 5 hours ( From 01.00 PM to 06.00 PM ).',
          'Format File NPM.pdf',
          'Test questions will be given at 01.00 PM and submission link will be closed at 06.00 PM'
        ],
        link_upload_jawaban: 'https://www.dropbox.com/request/4oxps8nqEqri1BTBLHJJ'
      },
      {
        color: 'brown',
        icon: 'mdi-flag',
        title: 'Elimination Section',
        date: '6 February 2020',
        descs: [
          'After going through 2 stages of registration with various assessments, you will be invited to Line multichat to proceed into final assessment.'
        ]
      },
      {
        color: 'indigo',
        icon: 'mdi-buffer',
        title: 'On-the-ground Assessment.',
        date: '10 February 2020',
        descs: [
          'Lecture Simulation.',
          'Face-to-face Interview.',
          'Coding test.'
        ],
        desc_det: 'Further assessment, this is the main part of your application, you will be test based your skills & knowledge in programming and other skills.'
      },
      {
        color: 'orange',
        icon: 'mdi-medal',
        date: '15 February 2020',
        title: 'Result Announcement.',
        descs: [
          'Please check Laboratory Assistant Line Official Account for the result.'
        ]
      }
    ]
  })
}
</script>
