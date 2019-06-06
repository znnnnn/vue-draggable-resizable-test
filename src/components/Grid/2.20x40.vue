<template>
  <!-- 网格20x40像素
  一个基本组件，grid=[20,40]prop用于设置网格单元的尺寸（高度和宽度，以像素为单位）。 -->
  <vue-draggable-resizable :grid="[20,40]">
    <p>Grid 20x40 starting from the top-left corner</p>
  </vue-draggable-resizable>
</template>
