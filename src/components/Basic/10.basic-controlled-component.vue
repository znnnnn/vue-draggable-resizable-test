<template>
  <vue-draggable-resizable :x="x"
                           :y="y"
                           :w="w"
                           :h="h"
                           @resizing="onResize"
                           @dragging="onDrag">
    <p>Basic controlled component.</p>
    <p>
      x: <input v-model.number="x" type="number">
    </p>
    <p>
      y: <input v-model.number="y" type="number">
    </p>
    <p>
      w: <input v-model.number="w" type="number">
    </p>
    <p>
      h: <input v-model.number="h" type="number">
    </p>
  </vue-draggable-resizable>
</template>


<script>
export default {
  data() {
    return {
      x: 0, y: 0, w: 200, h: 200
    }
  },
  methods: {
    onDrag(left, top) {
      this.x = left
      this.y = top
    },
    onResize(left, top, width, height) {
      this.x = left
      this.y = top
      this.w = width
      this.h = height
    }
  }
}
</script>