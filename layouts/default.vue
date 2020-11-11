<template>
  <v-app dark>
    <v-navigation-drawer
      mini-variant
      mini-variant-width="63"
      fixed
      app
      permanent
    >
      <v-list style="padding-top: 0">
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
          style="padding: 5px"
        >
          <v-list-item-content>
            <v-icon>{{ item.icon }}</v-icon>
            <v-list-item-title
              style="font-size: 11px; white-space: normal; text-align: center"
              v-text="item.title"
            />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar fixed app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <v-btn icon @click.stop="miniVariant = !miniVariant">
        <v-icon>mdi-{{ `chevron-${miniVariant ? 'right' : 'left'}` }}</v-icon>
      </v-btn>
      <v-btn icon @click.stop="clipped = !clipped">
        <v-icon>mdi-application</v-icon>
      </v-btn>
      <v-btn icon @click.stop="fixed = !fixed">
        <v-icon>mdi-minus</v-icon>
      </v-btn>
      <v-toolbar-title v-text="title" />
      <v-spacer />
      <v-btn icon @click.stop="rightDrawer = !rightDrawer">
        <v-icon>mdi-menu</v-icon>
      </v-btn>
    </v-app-bar>
    <v-main>
      <v-col
        style="
          width: 215.15px;
          height: calc(100% - 64px);
          position: fixed;
          background: green;
          overflow-y: auto;
        "
        v-if="drawer"
      >
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
        <v-list-item-content>
          <v-icon>mdi-calendar</v-icon>
        </v-list-item-content>
      </v-col>
      <v-container :style="drawer ? 'padding-left: 200px' : ''">
        <nuxt />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-calendar',
          title: 'Welcome',
          to: '/',
        },
        {
          icon: 'mdi-chart-pie',
          title: 'Inspire',
          to: '/inspire',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js',
    }
  },
}
</script>
<style>
::-webkit-scrollbar-thumb {
  border-radius: 100px;
  background-color: #cfd8dc;
  border: 3px solid #fff;
}
::-webkit-scrollbar {
    width: 7px!important;
}
</style>
