<template>
  <!-- 父母的组件成本
  无法在其父元素之外拖动或调整大小的组件，使用prop定义:parent="true"。 -->
  <vue-draggable-resizable :parent="true">
    <p>You cannot move or resize me outside my parent element.</p>
  </vue-draggable-resizable>
</template>
