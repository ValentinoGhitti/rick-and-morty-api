<template>
    <div class="btn-group" role="group" aria-label="Basic example">
        <button type="button" class="btn btn-dark"  @click="filter('')">All</button>
        <button type="button" class="btn btn-dark" @click="filter('Alive')">Alive</button>
        <button type="button" class="btn btn-dark" @click="filter('Dead')">Dead</button>
        <button type="button" class="btn btn-dark" @click="filter('unknown')">Unknown</button>
    </div>
</template>

<script>
import { useStore } from 'vuex'
export default {
    setup() {
        const store = useStore()
        const filter = ((status) => {
            store.dispatch('filterByStatus', status)
        })
        return {filter}
    }
}
</script>

<style>
.item {
    margin: 20px;
    cursor: pointer;
}
</style>