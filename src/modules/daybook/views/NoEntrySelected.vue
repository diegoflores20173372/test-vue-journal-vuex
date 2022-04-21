<template>
  <div class="d-flex justify-content-center">
    <h1 class="align-self-center">No hay nada seleccionado</h1>
  </div>

  <FabEntry />
</template>

<script>
import {defineAsyncComponent} from "vue";

export default {
  name: "NoEntrySelected",
  components: {
    FabEntry: defineAsyncComponent(() => import('../components/FabEntry'))
  }
}
</script>

<style lang="scss" scoped>
div{
  height: 100%;
}
</style>