<template>
  <vue-draggable-resizable>
    <input v-model="text" type="text">
    <input type="button" value="submit"
           @click="inputAlert">
  </vue-draggable-resizable>
</template>

<script>
export default {
  data() {
    return {
      text: ''
    }
  },
  methods: {
    inputAlert() {
      alert(this.text)
    }
  }
}
</script>

