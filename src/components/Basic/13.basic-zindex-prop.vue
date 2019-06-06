<template>
  <vue-draggable-resizable :z-index="zindex">
    <p>Controlling the z-index from outside the component by providing the <b>:z</b> prop.</p>
  </vue-draggable-resizable>
</template>

<script>
export default {
  data() {
    return {
      zindex: 1
    }
  },
}
</script>