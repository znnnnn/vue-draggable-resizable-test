<template>
  <!-- 轴支撑的基本组件
一个基本组件，axis支持控制哪个轴可拖动。合适的值是x，y或both。 -->
  <vue-draggable-resizable :axis="axis">
    <p>Draggable on {{axis}} axis.</p>
  </vue-draggable-resizable>
</template>

<script>
export default {
  data() {
    return {
      axis: 'y' // x / both
    }
  },
}
</script>