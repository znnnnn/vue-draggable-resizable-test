<template>
  <!-- 您可以使用handlesprop接受一个句柄数组来选择要为组件提供的句柄。例如，如果要仅在水平轴上进行尺寸调整，则只能提供左右手柄:handles="['ml','mr']"。 -->
  <!-- <vue-draggable-resizable :prevent-deactivation="true" :handles="['tl','tm','tr','mr','br','bm','bl','ml']"> -->
  <vue-draggable-resizable :prevent-deactivation="true" :handles="['tl','tm']">
    <p>Enable/disable handles.</p>
  </vue-draggable-resizable>
</template>
