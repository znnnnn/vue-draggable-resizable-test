<template>
  <!-- 组件不可调整大小
一个基本组件，resizableprop设置为false，因此它不可调整大小。 -->
  <vue-draggable-resizable :resizable="true">
    <p>Basic component that is not resizable.</p>
  </vue-draggable-resizable>
</template>
