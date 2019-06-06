<template>
  <!-- 具有主动控制的基本组件
一个基本组件，具有active从组件外部控制活动状态的prop。 -->
  <vue-draggable-resizable :active.sync="active">
    <p>Controlling the active state from outside the component by providing the <b>:active</b> prop.</p>
  </vue-draggable-resizable>
</template>

<script>
export default {
  data() {
    return {
      active: false
    }
  },
}
</script>