<template>
  <p>{{ msg }} : {{ msg2 }}</p>
  <!-- eslint-disable-next-line vue/require-component-is -->
  <Component v-model:msg="msg" v-model:msg2="msg2" />
</template>

<script>
import Component from './Component.vue'
export default {
  data() {
    return {
      msg: '초기 메세지',
      msg2: '초기 메세지',
    }
  },
  components: {
    Component,
  },
}
</script>
