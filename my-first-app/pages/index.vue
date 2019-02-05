<template>
  <v-layout
    column
    justify-center
    nothing

  >
    <!--<v-flex-->
      <!--xs50-->
      <!--sm8-->
      <!--md2-->
    <!--&gt;-->
      <div class="text-xs-center">
        <logo />
        <vuetify-logo />
      </div>
      <v-card>
          <!--<v-card-title class="headline">Welcome to the paradise to find the special person.</v-card-title>-->
        <v-card-text>
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            f="circle"
            nuxt
            to="/Homepage"
          >Countinue</v-btn>
          <v-btn fab drepressed  dark color="purple">
            <v-icon>email</v-icon>
          </v-btn>
        </v-card-actions>

      </v-card>

    <!--</v-flex>-->
  </v-layout>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {
    Logo,
    Logo
  }
}
</script>
