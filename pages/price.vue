<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <v-card>
        <v-card-title>通常料金</v-card-title>
        <v-divider></v-divider>
        <v-data-table
          :headers="headers"
          :items="items"
          :hide-default-footer="true"
          :disable-sort=true
        >
        </v-data-table>
      </v-card>
      <padding-line></padding-line>
      <v-card>
        <v-card-title>オープン記念（限定10社）</v-card-title>
        <v-divider></v-divider>
        <v-data-table
          :headers="headers"
          :items="items"
          :hide-default-footer="true"
          :disable-sort=true
        >
        </v-data-table>
      </v-card>
    </v-col>
  </v-row>
</template>

<script src="vue.js"></script>
<script src="vuetify.js"></script>

<script>
import PaddingLine from '~/components/PaddingLine.vue'
export default {
  data: () => ({
    windowWidth: 0,
    mobileScreenWidth: 600,
    headers: [
      { text: '内容', align: 'center', sortable: false, value: 'name' },
      { text: '料金［ 円 ］', align: 'center', value: 'price' },
    ],
    items: [
      { name: '相談・お見積り', price: '無料' },
      { name: '初期導入', price: '30,000' },
      { name: '月額', price: '10,000' },
    ],
  }),
}
</script>
