<template>
  <!-- 具有宽高比的组件
一个组件，lock-aspect-ratioprop用于在调整大小期间保持组件的宽高比。 -->

  <vue-draggable-resizable :lock-aspect-ratio="true">
    <p>Keep aspect ratio using <b>:lock-aspect-ratio</b> prop.</p>
  </vue-draggable-resizable>
</template>
