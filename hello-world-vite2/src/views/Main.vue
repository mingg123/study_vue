<template>
  <h1>main page</h1>
  <!-- {{ dummy }} -->
  <div v-for="(value, key) in label" :key="key">
    {{ value }} : {{ dummy[value] }}
  </div>
</template>

<script>
import { defineComponent } from 'vue';
import dummy from './dummy';
export default defineComponent({
  data() {
    return {
      dummy: dummy,
      label: ['아파트명', '지역평단가', '면적', '실거래가'],
    };
  },
});
</script>
