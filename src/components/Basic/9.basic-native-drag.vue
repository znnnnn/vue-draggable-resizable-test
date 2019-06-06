<template>
  <!-- 一个基本组件，enable-native-dragprop设置为true，以允许本机浏览器的拖动行为。您可以通过使用球拖动每个组件来查看差异。默认值是false。 -->
  <vue-draggable-resizable :enable-native-drag="true">
    <p>Native drag enabled. Try to drag the component from the ball.</p>
    <img src="@/assets/logo.png" alt="">
  </vue-draggable-resizable>
</template>
