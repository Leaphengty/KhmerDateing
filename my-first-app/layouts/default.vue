<template>
  <v-app class="pink">
    <!--<v-navigation-drawer-->
      <!--v-model="drawer"-->
      <!--:mini-variant="miniVariant"-->
      <!--:clipped="clipped"-->
      <!--app-->
    <!--&gt;-->
      <!--<v-list>-->
        <!--<v-list-tile-->
          <!--v-for="(item, i) in items"-->
          <!--:key="i"-->
          <!--:to="item.to"-->
          <!--router-->
          <!--exact-->
        <!--&gt;-->
          <!--&lt;!&ndash;<v-list-tile-action>&ndash;&gt;-->
            <!--&lt;!&ndash;<v-icon>{{ item.icon }}</v-icon>&ndash;&gt;-->
          <!--&lt;!&ndash;</v-list-tile-action>&ndash;&gt;-->
          <!--<v-list-tile-content>-->
            <!--<v-list-tile-title v-text="item.title" />-->
          <!--</v-list-tile-content>-->
        <!--</v-list-tile>-->
      <!--</v-list>-->
    <!--</v-navigation-drawer>-->
    <!--<v-toolbar-->
      <!--:clipped-left="clipped"-->
      <!--fixed-->
      <!--app-->
    <!--&gt;-->
      <!--<v-toolbar-side-icon @click="drawer = !drawer" />-->
      <!--<v-btn-->
        <!--icon-->
        <!--@click.stop="miniVariant = !miniVariant"-->
      <!--&gt;-->
        <!--<v-icon>{{ `chevron_${miniVariant ? 'right' : 'left'}` }}</v-icon>-->
      <!--</v-btn>-->
      <!--<v-btn-->
        <!--icon-->
        <!--@click.stop="clipped = !clipped"-->
      <!--&gt;-->
        <!--<v-icon>web</v-icon>-->
      <!--</v-btn>-->
      <!--<v-btn-->
        <!--icon-->
        <!--@click.stop="fixed = !fixed"-->
      <!--&gt;-->
        <!--<v-icon>remove</v-icon>-->
      <!--</v-btn>-->
      <!--<v-toolbar-title v-text="title" />-->
      <!--<v-btn-->
        <!--icon-->
        <!--@click.stop="rightDrawer = !rightDrawer"-->
      <!--&gt;-->
        <!--<v-icon>menu</v-icon>-->
      <!--</v-btn>-->

    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>
    <!--<v-navigation-drawer-->
      <!--v-model="rightDrawer"-->
      <!--:right="right"-->
      <!--temporary-->
      <!--fixed-->
    <!--&gt;-->
      <!--&lt;!&ndash;<v-list>&ndash;&gt;-->
        <!--&lt;!&ndash;<v-list-tile @click.native="right = !right">&ndash;&gt;-->
          <!--&lt;!&ndash;<v-list-tile-action>&ndash;&gt;-->
            <!--&lt;!&ndash;<v-icon light>compare_arrows</v-icon>&ndash;&gt;-->
          <!--&lt;!&ndash;</v-list-tile-action>&ndash;&gt;-->
          <!--&lt;!&ndash;<v-list-tile-title>Switch drawer (click me)</v-list-tile-title>&ndash;&gt;-->
        <!--&lt;!&ndash;</v-list-tile>&ndash;&gt;-->
      <!--&lt;!&ndash;</v-list>&ndash;&gt;-->
    <!--</v-navigation-drawer>-->
    <v-footer class="pink center--text"
      app
    >
      <span alr>&copy;copy right KhmerDating</span>
    </v-footer>
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
          icon: 'apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'bubble_chart',
          title: 'Inspire',
          to: '/Homepage'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      // title: 'Vuetify.js'
      title:'KhmerDating',
      color: 'pink'
    }
  }
}
</script>
