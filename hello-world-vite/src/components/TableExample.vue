<template>
  <table>
    <tr>
      <th v-for="(head, head_index) in header" :key="head_index">
        {{ head }}
      </th>
    </tr>
    <tr v-for="(row, index) in rows" :key="index">
      <td
        v-for="(data, rowIndex) in row"
        :key="rowIndex"
        :colspan="data.colspa || 1"
      >
        {{ data.data }}
      </td>
    </tr>

    <!-- <tr>
      <th>1번 제목</th>
      <th>2번 제목</th>
    </tr>
    <tr>
      <td>1번 내용</td>
      <td>2번 내용</td>
    </tr>
    <tr>
      <td>1번 내용</td>
      <td>2번 내용</td>
    </tr> -->
  </table>
</template>

<script>
export default {
  props: ['header', 'rows'],
  // data() {
  //   const table = {
  //     header: ['1번 제목', '2번 제목'],
  //     rows: [
  //       [{ data: '1번 제목' }, { data: '2번 제목' }],
  //       [{ data: '1번 내용2', colspan: 2 }],
  //     ],
  //   }
  //   return table
  // },
}
</script>

<style scoped>
table,
th,
td {
  border: 1px solid black;
  border-collapse: collapse;
  padding: 5px;
}
</style>
