<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <v-card>
        <v-card-title class="headline">
          リッチメニューカスタマイズ
        </v-card-title>
        <v-card-text>
          <div class="text-center">
            <rich-menu/>
          </div>
          <p>リッチメニューを自由にカスタマイズ！タブ切り替えでまるでサイトのように使うことができます！</p>
        <hr class="my-3">
             <padding-line></padding-line>
  <v-row justify="center" align="center">
            <v-btn
    color="primary"
    to='/richamenu-service'
    target="_self"
  >
    詳細
  </v-btn>
  <padding-line></padding-line>
  </v-row>
        </v-card-text>
      </v-card>
     <padding-line></padding-line>
      <v-card>
        <v-card-title class="headline">
          Lステップ（LINEのステップ配信）
        </v-card-title>
        <v-card-text>
          <p>特定のターゲットに向けてステップ配信が可能！
            <br>
            ステップ配信とは、一斉配信とは異なるストーリーに沿った配信のことです。
          </p>
          <hr class="my-3" >
               <padding-line></padding-line>
  <v-row justify="center" align="center">
            <v-btn
    color="primary"
    target="_blank"
    disabled
  >
    近日公開
  </v-btn>
  </v-row>
        </v-card-text>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
import RichMenu from '~/components/RichMenu.vue'
export default {
  components: {
RichMenu
  }
}
</script>
