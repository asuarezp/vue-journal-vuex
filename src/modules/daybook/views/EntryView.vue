<template>
  <div class="entry-title d-flex justify-content-between p-2">
    <div>
        <span class="text-success fs-3 fw-bold">20</span>
        <span class="mx-1 fs-3">November</span>
        <span class="mx-2 fs-4 fw-light">2023, Monday</span>
    </div>

    <div>
        <button class="btn btn-danger mx-2">
            Borrar
            <i class="fa fa-trash-alt"></i>
        </button>
        <button class="btn btn-primary">
            Subir foto
            <i class="fa fa-trash-upload"></i>
        </button>
    </div>
  </div>

  <hr>

  <div class="d-flex flex-column px-3 h-75">
    <textarea 
        placeholder="¿Qué sucedió hoy?"
        ></textarea>
  </div>

  <fa-b icon="fa-save"></fa-b>

  <img  src="https://picsum.photos/id/13/2500/1667" 
        alt="entry-picture"
        class="img-thumbnail"
  >
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

textarea {
    font-size: 20px;
    border: none;
    height: 100%;

    &:focus {
        outline: none;
    }
}

img {
    width: 200px;
    position: fixed;
    bottom: 150px;
    right: 20px;
    box-shadow: 0px 5px 10px rgba($color: #000000, $alpha: 0.2);
}
</style>