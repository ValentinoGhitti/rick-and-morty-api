<template>
    <section class="d-flex justify-content-center bg-light">
        <div class="characters bg-light d-flex flex-wrap justify-content-center mb-5">
            <div class="characters-item" v-for="character in characters" :key="character.id">
                <Card :character="character" />
            </div>
        </div>
        <div v-if="characters.length == 0" class="d-flex flex-column justify-content-center mt-5 mb-5 ">
            <div class="d-flex justify-content-center"> 
                <img class="gif" src="../../public/img/morty.gif" alt="wrong-name">
            </div>
            <h5>Character not found </h5>
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

<style scoped>
    .gif {
        width: 130px;
    }
</style>