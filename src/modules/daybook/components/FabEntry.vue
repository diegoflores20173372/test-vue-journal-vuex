<template>
  <button class="btn btn-primary">
    <i class="fa fa-2x" :class="iconFab"></i>
  </button>
</template>

<script>
export default {
  name: "FabEntry",
  computed: {
    iconFab() {
      if (this.$route.params.id) {
        return 'fa-save'
      } else {
        return 'fa-plus'
      }
    }
  }
}
</script>

<style lang="scss" scoped>
button {
  position: fixed;
  bottom: 20px;
  right: 20px;
  width: 80px;
  height: 80px;
  border-radius: 100%;
}
</style>