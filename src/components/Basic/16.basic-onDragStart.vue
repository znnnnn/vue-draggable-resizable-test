<template>
  <!-- onDragStart回调的基本组件
一个基本组件，onDragStartprop用于接受在拖动开始时调用的函数（单击或触摸元素）。如果函数返回false，则取消操作。您可以使用此功能来防止事件冒泡。 -->

  <vue-draggable-resizable :on-drag-start="onDragStartCallback">
    <p>Passing a callback to the component that gets called as soon as the component is clicked.</p>
  </vue-draggable-resizable>
</template>

<script>
export default {
  methods: {
    onDragStartCallback: function() {
      alert(1)
    }
  }
}
</script>
