<template>
  <div class="d-flex justify-content-center">
    <h1 class="align-self-center">No hay nada seleccionado</h1>
  </div>
  <fa-b icon="fa-plus"></fa-b>
</template>

<script>
import { defineAsyncComponent } from 'vue'

export default {
    components: {
        FaB: defineAsyncComponent(() => import('../components/FaB.vue'))
    }
}
</script>

<style lang="scss" scoped>
div {
    height: 100%;
}
</style>