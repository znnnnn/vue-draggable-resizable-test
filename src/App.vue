<template>
  <div id="app">
    <div class="container">
      <test></test>
    </div>
  </div>
</template>

<script>
import test from './components/Aspect Radio/1.basic'

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
* {
  margin: 0;
  padding: 0;
}

.container {
  box-sizing: border-box;
  border: 2px solid #000;
  width: 1000px;
  height: 500px;
  background: linear-gradient(-90deg, rgba(0, 0, 0, 0.1) 1px, transparent 1px)
      20px 200px / 20px 20px,
    linear-gradient(rgba(0, 0, 0, 0.1) 1px, transparent 1px) 0% 0% / 20px 20px;
}
</style>