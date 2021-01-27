<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <v-card>
        <v-card-title>お問い合わせ</v-card-title>
        <v-card-text justify="center" align="center">
                  <question-button/>
          </v-card-text>
      </v-card>
    </v-col>
  </v-row>
</template>


<script>
import TempLogo from '~/components/TempLogo.vue'
import QuestionButton from '~/components/QuestionButton.vue'

export default {
  components: {
    TempLogo,
    QuestionButton
  }
}
</script>
