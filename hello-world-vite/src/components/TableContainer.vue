<template>
  <MyTable :header="header" :rows="rows" />
</template>

<script>
import MyTable from './TableExample.vue'

export default {
  name: 'TableContainer',
  data() {
    return {
      header: ['1번 제목', '2번 제목'],
      rows: [
        [{ data: '1번 제목' }, { data: '2번 제목' }],
        [{ data: '1번 내용2', colspan: 2 }],
      ],
    }
  },
  components: {
    MyTable,
  },
}
</script>
