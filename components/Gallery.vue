<template>
  <v-sheet
    class="mx-auto"
    style="background-color: #fafafa;"
  >
    <v-slide-group
      v-model="item"
      class="pa-4"
      center-active
      show-arrows
    >
      <v-slide-item
        v-for="(item, i) in items"
        :key="i"
        v-slot:default="{ active, toggle }"
      >
        <v-card
          :color="active ? 'primary' : 'grey lighten-1'"
          class="ma-4"
          height="200"
          width="100"
          @click="toggle"
        >
          <v-img
            :src="item.url"
            aspect-ratio="0.5"
          >
          </v-img>
        </v-card>
      </v-slide-item>
    </v-slide-group>
    <v-row
      class="body-1"
      justify="center"
    >
      <blockquote class="blockquote text-center">
        <p>Register now to be a part of our big family.</p>
        <p>Gain all the benefits and valuable experience in your life!</p>
        <p class="title">-Laboratory Assistant 2019</p>
      </blockquote>
    </v-row>
  </v-sheet>
</template>

<script>
export default {
  data: () => ({
    item: 1,
    items: [
      { url: 'Gallery/achun.jpg' },
      { url: 'Gallery/argil.jpg' },
      { url: 'Gallery/caca.jpg' },
      { url: 'Gallery/agnes.jpg' },
      { url: 'Gallery/dilla.jpg' },
      { url: 'Gallery/mansyah.jpg' },
      { url: 'Gallery/marcell.jpg' },
      { url: 'Gallery/abay.jpg' },
      { url: 'Gallery/afifah.JPG' },
      { url: 'Gallery/baby.jpg' },
      { url: 'Gallery/dzakia.jpg' },
      { url: 'Gallery/eko.jpg' },
      { url: 'Gallery/fahmi.jpg' },
      { url: 'Gallery/radit.jpg' },
      { url: 'Gallery/syifa.jpg' },
      { url: 'Gallery/vega.jpg' }
    ]
  })
}
</script>
