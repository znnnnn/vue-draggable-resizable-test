<template>
  <div style="height: 500px; width: 500px; border: 1px solid red; position: relative;">
    <vue-draggable-resizable :w="200"
                             :h="200"
                             @dragging="onDrag"
                             @dragstop="onDragStop">
      <p>{{dragging ? 'You are dragging me crazy' : 'Standing still'}}</p>
      <p>{{x}},{{y}}</p>
    </vue-draggable-resizable>
  </div>
</template>

<script>
export default {
  name: 'app',
  components: {
  },
  data() {
    return {
      x: 0,
      y: 0,
      dragging: false
    }
  },
  methods: {
    onDrag: function (x, y) {
      this.dragging = true
      this.x = x
      this.y = y
    },
    onDragStop: function (x, y) {
      console.log(x, y)
      this.dragging = false
    }
  }
}
</script>