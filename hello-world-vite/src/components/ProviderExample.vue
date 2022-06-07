<template>
  <!-- eslint-disable-next-line vue/require-component-is -->
  <Component />
</template>

<script>
import Component from './Component.vue'
import { provide } from 'vue'

export default {
  provide: {
    msg: '메시지',
  },
  components: {
    Component,
  },
}
</script>
