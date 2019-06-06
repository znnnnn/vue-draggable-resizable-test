<template>
  <vue-draggable-resizable :on-resize-start="onResizeStartCallback">
    <p>Passing a callback to the component that gets called as soon as the component is resized.</p>
  </vue-draggable-resizable>
</template>

<script>
export default {
  methods: {
    onResizeStartCallback: function() {
      console.log(1)
    }
  }
}
</script>