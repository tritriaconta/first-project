<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <div class="text-center">
        <tritri-logo/>
      </div>
      <v-card>
        <v-card-title class="headline">
          情報
        </v-card-title>
        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title>担当</v-list-item-title>
            <v-list-item-subtitle>よっしー</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title>活動開始</v-list-item-title>
            <v-list-item-subtitle>2021/03/03</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title></v-list-item-title>
            <v-list-item-subtitle></v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
import TritriLogo from '~/components/TritriLogo.vue'
export default {
  components: {
    TritriLogo
  }
}
</script>
