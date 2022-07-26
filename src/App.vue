<template>
  <Nav :class="{'d-none': scrollPosition > 400}" ></Nav>
  <Main id="welcome"></Main>
  <div class="container">
    <FilterByName />
    <CharactersList />
  </div>
  <Footer></Footer>
</template>

<script>
import Main from './components/Main.vue'
import Nav from './components/Nav.vue'
import Footer from './components/Footer.vue'
import FilterByName from './components/FilterByName.vue'
import CharactersList from '../src/components/CharactersList.vue'
export default {
  name: 'App',
  components: {
    CharactersList,
    FilterByName,
    Main,
    Nav,
    Footer
  },
  data() {
    return {
      scrollPosition: null
    }
  },
  methods: {
    updateScroll() {
      this.scrollPosition = window.scrollY
    }
  },
  mounted() {
    window.addEventListener('scroll', this.updateScroll)
  }
}
</script>