<template>
  <vue-draggable-resizable :w="200"
                           :h="200"
                           @activated="onActivated"
                           @deactivated="onDeactivated">
    <p v-if="active">The component has been activated.</p>
  </vue-draggable-resizable>
</template>


<script>
export default {
  data() {
    return {
      active: false
    }
  },
  methods: {
    onActivated() {
      this.active = true
    },
    onDeactivated() {
      this.active = false
    }
  }
}
</script>