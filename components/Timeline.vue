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
              v-for="(desc) in item.descs"
            >
              {{ desc.poin }}
            </li>
          </ul>
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
        title: 'Make sure your\'e fit the requirements.',
        descs: [
          { poin: 'Anggota Penuh Himatif FMIPA Unpad and currently in third year (2016) or second year (2017).' },
          { poin: 'Minimum GPA 3.00.' },
          { poin: 'Have minimum grade B for the subject you wanted.' }
        ]
      },
      {
        color: 'purple',
        icon: 'mdi-book-variant',
        title: 'Registration & Pre-screening Assessment.',
        date: '17 January 2020 - 31 January 2020',
        descs: [
          { poin: 'Register yourself, fill the form. ' },
          { poin: 'Upload the requirement files (CV, Cover Letter) in pdf files.' },
          { poin: 'Upload your Academic Transcript (jpg/jpeg).' },
          { poin: 'Submit Instagram links for short introduction video.' }
        ]
      },
      {
        color: 'green',
        icon: 'mdi-laptop',
        title: 'Online Assessment.',
        date: '2 February 2020 - 4 February 2020',
        descs: [
          { poin: 'A test for your basic skills, you will be given a chance to answer some questions.' }
        ]
      },
      {
        color: 'indigo',
        icon: 'mdi-buffer',
        title: 'On-the-ground Assessment.',
        date: '10 February 2020',
        descs: [
          { poin: 'Lecture Simulation.' },
          { poin: 'Face-to-face Interview.' },
          { poin: 'Coding test.' }
        ],
        desc_det: 'Further assessment, this is the main part of your application, you will be test based your skills & knowledge in programming and other skills.'
      },
      {
        color: 'orange',
        icon: 'mdi-flag',
        date: '15 February 2020',
        title: 'Result Announcement.',
        descs: [
          { poin: 'Please check Laboratory Assistant Official Account for the result.' }
        ]
      }
    ]
  })
}
</script>
