<template>
  <v-app light>
    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      app
    >
    <v-btn
      @click.stop="clipped = !clipped"
      icon
    >
      <v-icon>mdi-application</v-icon>
    </v-btn>
    <v-btn
      @click.stop="miniVariant = !miniVariant"
      icon
    >
      <v-icon>mdi-{{ `chevron-${miniVariant ? 'right' : 'left'}` }}</v-icon>
    </v-btn>
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar
      :clipped-left="clipped"
      :collapse-on-scroll="false"
      elevate-on-scroll
      inverted-scroll
      fixed
      dense
      app
    >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <v-toolbar-title v-text="title" />
    </v-app-bar>
    <v-content>
      <v-container
        fluid
        ma-0
        pa-0
      >
        <nuxt />
      </v-container>
    </v-content>
    <v-footer
      absolute
      :width="100"
      app
    >
      <span><a href="https://github.com/atjhoendz" target="_blank" style="color:black; text-decoration:none"> &copy; 2020</a></span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-home',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Requirements',
          to: '/requirements'
        },
        {
          icon: 'mdi-lamp',
          title: 'FAQ',
          to: 'faq'
        }
      ],
      miniVariant: true,
      title: 'oprecastprak2020'
    }
  }
}
</script>
