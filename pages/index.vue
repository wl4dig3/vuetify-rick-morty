<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <div class="text-center">
        <logo />
        <vuetify-logo />
      </div>
      <v-card>
        <v-card-title class="headline">
          Welcome to this little nuxt-vuetify practice
        </v-card-title>
        <v-card-text>
          <p>Kindly click 'barra' link at the left to get to the characters</p>
          
          
          
          <p>Thank you for seeing this little proyect.</p>
          <div class="text-xs-right">
            <em><small>&mdash; Wladimir Guevara</small></em>
          </div>
          <hr class="my-3">
          
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'


export default {
  components: {
    Logo,
    VuetifyLogo
  }
  
}
</script>
