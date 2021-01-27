<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <!-- <div class="text-center">
        <jump-img/>
      </div>      -->
      <v-card>
        <v-card-title class="headline">
          L-JUMP （エルジャンプ）
        </v-card-title>
        <v-card-text>
          <p>これからのマーケティングにはLINE公式アカウントの運用が必須！
            公式アカウントのリッチメニューやLINEのステップ配信Lステップを強力にサポート！
            <br><br>
            Lステップを使いこなし、事業を格段にジャンプさせます！L公式を使いこなしホップ・ステップ・ジャンプ！            
          </p>
          <!-- <p>
            If you have questions, please join the official <a
              href="https://chat.vuetifyjs.com/"
              target="_blank"
              rel="noopener noreferrer"
              title="chat"
            >
              discord
            </a>.
          </p> -->
          <!-- <p>
            Find a bug? Report it on the github <a
              href="https://github.com/vuetifyjs/vuetify/issues"
              target="_blank"
              rel="noopener noreferrer"
              title="contribute"
            >
              issue board
            </a>.
          </p> -->
          <!-- <p>Thank you for developing with Vuetify and I look forward to bringing more exciting features in the future.</p>
          <div class="text-xs-right">
            <em><small>&mdash; John Leider</small></em>
          </div> -->
          <hr class="my-3">
      <div class="text-center">
          <p>
            こちらからお気軽にご連絡ください。
            <br>
          <question-button/>
          </p>
      </div>     
          <br>
          <!-- <a
            href="https://github.com/nuxt/nuxt.js"
            target="_blank"
            rel="noopener noreferrer"
          >
            Nuxt GitHub
          </a> -->
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <!-- <v-btn
            color="primary"
            nuxt
            to="/inspire"
          >
            問合せ
          </v-btn> -->
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
// import JumpImg from '~/components/JumpImg.vue'
import TempTab from '~/components/Tab.vue'
import QuestionButton from '~/components/QuestionButton.vue'

export default {
  components: {
    TempTab,
    QuestionButton
  }
}
</script>
