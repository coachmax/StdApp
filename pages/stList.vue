<template>
  <v-data-table
    :headers="headers"
    :items="items"
    hide-actions
    class="elevation-1"
  >
    <template slot="items" slot-scope="props">
      <td>{{ props.item.code }}</td>
      <td class="text-xs-right">{{ props.item.name }}</td>
      <td class="text-xs-right">{{ props.item.group }}</td>
      <td class="text-xs-right">{{ props.item.carbs }}</td>
      <td class="text-xs-right">{{ props.item.protein }}</td>
      <td class="text-xs-right">{{ props.item.iron }}</td>
    </template>
  </v-data-table>
</template>
<script>
  export default {
      layout: 'member',
    data () {
      return {
        headers: [
          {
            text: 'รหัสนักศึกษา',
            align: 'left',
            sortable: false,
            value: 'name'
          },
          { text: 'ชื่อ-สกุล', value: 'calories' },
          { text: 'กลุ่ม', value: 'group' },
          { text: 'พฤติกรรม', value: 'carbs' },
          { text: 'รายการ', value: 'protein' }
        ],
        items: [
          {
            value: false,
            code: '613204001',
            name: 'สมชาย ใจดี',
            group: 'พณค.11',
            carbs: 'เก็บเงินได้',
            protein: '+5'
          },
          {
            value: false,
            code: '613204002',
            name: 'สมหมาย ใจปอง',
            group: 'พณค.11',
            carbs: 'ผมยาว',
            protein: '-5'
          },
          {
            value: false,
            code: '613204003',
            name: 'สมพิศ พิษเยอะ',
            group: 'พณค.11',
            carbs: 'ผมยาว',
            protein: '-5'
          },
          {
            value: false,
            code: '613204004',
            name: 'สมหมาย ใจปอง',
            group: 'พณค.11',
            carbs: 'ผมยาว',
            protein: '-5'
          },
          {
            value: false,
            code: '613204005',
            name: 'สมหมาย ใจปอง',
            group: 'พณค.11',
            carbs: 'ผมยาว',
            protein: '-5'
          },
          {
            value: false,
            name: '613204006',
            calories: 'สมปอง ใจดี',
            group: 'พณค.11',
            carbs: 'ผมยาว',
            protein: '-5'
          },
          {
            value: false,
            code: '613204007',
            name: 'สมหมาย ใจปอง',
            group: 'พณค.11',
            carbs: 'ผมยาว',
            protein: '-5'
          },
          {
            value: false,
            code: '613204008',
            name: 'สมหมาย ใจปอง',
            group: 'พณค.11',
            carbs: 'ผมยาว',
            protein: '-5'
          },
          {
            value: false,
            code: '613204009',
            name: 'สมหมาย ใจปอง',
            group: 'พณค.11',
            carbs: 'ผมยาว',
            protein: '-5'
          },
          {
            value: false,
            code: '6132040010',
            name: 'สมหมาย ใจปอง',
            group: 'พณค.11',
            carbs: 'ผมยาว',
            protein: '-5'
          }
        ]
      }
    }
  }
</script>