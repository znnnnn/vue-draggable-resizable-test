<template>
  <div id="app">
    <div style="height: 500px; width: 500px; border: 1px solid red; position: relative;">
      <test></test>
    </div>
  </div>
</template>

<script>
import test from './components/Events/Resizing'

export default {
  name: 'app',
  components: {
    test
  },
  data() {
    return {
    }
  },
  methods: {
  }
}
</script>

<style>
.vdr {
  border: 1px dashed black;
}
</style>