<template>
  <div @click="$router.push({ name: 'entry', params: { id: 10 }})" class="entry-container mb-3 pointer p-2">

    <div class="entry-title d-flex">
        <span class="text-success fx-5 fw-bold">20</span>
        <span class="mx-1 fs-5">November</span>
        <span class="mx-2 fw-light">2023, lunes</span>
    </div>

    <div class="entry-description">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Sit earum ullam dolor commodi laborum consequuntur. Ut quam, perferendis fugiat voluptates minima earum. Voluptate eum saepe distinctio quod, pariatur facilis rem!
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.entry-container {
    border-bottom: 1px solid #2c3e50;
    transition: 0.2s all ease-in;
    &:hover {
        background-color: lighten($color: grey, $amount: 45);
        transition: 0.2s all ease-in;
    }

    .entry-description {
        font-size: 12px;
    }
}
</style>