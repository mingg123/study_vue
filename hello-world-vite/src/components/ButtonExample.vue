<template>
  <MyButton sm>MyButton</MyButton>
  <MyButtonm>MyButton</MyButtonm>
  <MyButton lg background-white>MyButton</MyButton>
  <MyButton sm pill text-red background-black>MyButton</MyButton>
  <MyButton md pill text-red background-pink>MyButton</MyButton>
  <MyButton lg pill @click.prevent="onClick">MyButton</MyButton>
  <MyButton lg pill v-on:click="onClick">MyButton</MyButton>
</template>

<script>
import MyButton from './MyButton.vue'
export default {
  name: 'App',
  methods: {
    onClick(evt) {
      alert('Clicked')
    },
  },
  components: {
    MyButton,
  },
}
</script>
