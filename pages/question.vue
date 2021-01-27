<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <v-card>
        <v-card-title>お問い合わせ</v-card-title>
        <v-card-text justify="center" align="center">
                  <v-btn color="primary"
            href="https://forms.gle/vK6ReewgUusNJ79b8"
            target="_blank"
          >
          お問い合わせ
          </v-btn>
          </v-card-text>
      </v-card>
    </v-col>
  </v-row>
</template>


<script>
import TempLogo from '~/components/TempLogo.vue'
export default {
  components: {
    TempLogo
  }
}
</script>
