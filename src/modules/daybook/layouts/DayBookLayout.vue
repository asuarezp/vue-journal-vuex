<template>
    <the-navbar></the-navbar>

    <div class="d-flex">
        <div class="col-4">
            <EntryList />
        </div>
        <div class="col">
            <router-view />
        </div>
    </div>
</template>

<script>
import { defineAsyncComponent } from 'vue'

export default {
    components: {
        TheNavbar: defineAsyncComponent(() => import('../components/TheNavbar.vue')),
        EntryList: defineAsyncComponent(() => import('../components/EntryList.vue'))
    }
}
</script>