<template>
    <div class="container pt-5 bg-light ">
        <div class="d-flex justify-content-center mt-5 mb-5">
            <h2>List of Rick and Morty characters</h2>
        </div>
        <nav class="navbar bg-light">
            <div class="container-fluid search d-flex justify-content-around">
                <form @submit.prevent="filter()" id="characters" role="search">
                    <div class="p-3">
                        <h5 class="text-center" for="Search">Find character</h5>
                        <input 
                            class="form-control me-2" 
                            type="search" 
                            placeholder="Search" 
                            aria-label="Search"
                            v-model="name"
                            @keyup="filter()"
                        >
                    </div>
                    <div >
                        <FilterByStatusVue />
                    </div>
                </form>
            </div>
        </nav>
    </div>
</template>

<script>
import FilterByStatusVue from './FilterByStatus.vue'
import { ref } from 'vue'
import { useStore } from 'vuex'
export default {
    components: {
        FilterByStatusVue
    },
    setup() {
        const store = useStore()
        const name = ref('')
        const filter = () => {
            store.dispatch('filterByName', name.value)
        }
        return { name, filter}
    }
}
</script>

<style scoped>
h2 {
    font-family: get_schwifity;
}

</style>