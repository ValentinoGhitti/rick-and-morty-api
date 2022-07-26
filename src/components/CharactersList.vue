<template>
    <section>
        <div class="characters bg-light d-flex flex-wrap justify-content-center mb-5">
            <div class="characters-item" v-for="character in characters" :key="character.id">
                <Card :character="character" />
            </div>
        </div>
    </section>
</template>

<script>
import { onMounted, computed } from 'vue'
import { useStore } from 'vuex'
import Card from '../components/Card.vue'
export default {
    name: 'CharactersList',
    components: {
        Card
    },
    setup() {
        const store = useStore()
        const characters = computed(() => {
            return store.state.charactersFilter
        })
        onMounted(() => {
            store.dispatch('getCharacters')
        })
        return {characters}
    }
}
</script>