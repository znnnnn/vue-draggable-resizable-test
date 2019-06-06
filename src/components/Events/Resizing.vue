The resizing(x, y, width, height) event is emitted when the component is resized. The resizestop(x, y, width, height) event is emmitted when the resizing stops.

<template>
  <vue-draggable-resizable :w="200"
                           :h="200"
                           :x="0"
                           :y="0"
                           @resizing="onResize"
                           @resizestop="onResizeStop">
    <p>{{resizing ? 'You are resizing me crazy' : 'This is my favourite shape'}}</p>
    <p> {{x}},{{y}} </p>
    <p> {{width}},{{height}} </p>
  </vue-draggable-resizable>
</template>


<script>
export default {
  data() {
    return {
      x: 0,
      y: 0,
      width: 0,
      height: 0,
      resizing: false
    }
  },

  methods: {
    onResize: function (x, y, width, height) {
      this.resizing = true
      this.x = x
      this.y = y
      this.width = width
      this.height = height
    },
    onResizeStop: function (x, y, width, height) {
      this.resizing = false
    }
  }
}
</script>