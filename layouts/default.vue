<template>
  <v-app dark>
    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
    >
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
    <v-app-bar :clipped-left="clipped" fixed app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <v-btn icon @click.stop="miniVariant = !miniVariant">
        <v-icon>mdi-{{ `chevron-${miniVariant ? 'right' : 'left'}` }}</v-icon>
      </v-btn>
      <!-- <v-btn icon click.stop="clipped">
        <v-icon>mdi-application</v-icon>
      </v-btn> -->
      <!-- <v-btn icon @click.stop="fixed = !fixed">
        <v-icon>mdi-minus</v-icon>
      </v-btn> -->
      <v-toolbar-title v-text="title" />
      <v-spacer />
      <!-- <v-btn icon @click.stop="rightDrawer = !rightDrawer"> </v-btn> -->
    </v-app-bar>
    <v-main>
      <v-row justify="center" align="center">
        <v-col>
          <temp-tab></temp-tab>
        </v-col>
      </v-row>
      <v-container>
        <nuxt />
      </v-container>
    </v-main>
    <v-footer :absolute="!fixed" app>
      <span
        >Copyright &copy; {{ new Date().getFullYear() }} tritriaconta Co.,Ltd.
        All Rights Reserved</span
      >
    </v-footer>
  </v-app>
</template>

<script>
import TempTab from '~/components/Tab.vue'

export default {
  components: {
    TempTab,
  },
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-home',
          title: 'Home',
          to: '/',
        },
        {
          icon: 'mdi-cellphone',
          title: 'Service',
          to: '/service',
        },
        {
          icon: 'mdi-currency-usd',
          title: 'Price',
          to: '/price',
        },
        {
          icon: 'mdi-wechat',
          title: 'Question',
          to: '/question',
        },
        {
          icon: 'mdi-account',
          title: 'About',
          to: '/about',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'LINE公式アカウント運用サポートサービス L-JUMP',
    }
  },
}
</script>

<style lang="scss" scoped>
main {
  background-color:#d7fbe8;
}

footer{
  background-color:#1fab89;
}
</style>
