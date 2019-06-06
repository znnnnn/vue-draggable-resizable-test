<template>
  <!-- 一个基本组件，prevent-deactivation支持在外部点击时避免解除活动状态.. -->
  <vue-draggable-resizable :prevent-deactivation="true">
    <p>Prevents the deactivation of the component by providing the <b>:prevent-deactivation</b> prop.</p>
  </vue-draggable-resizable>
</template>
