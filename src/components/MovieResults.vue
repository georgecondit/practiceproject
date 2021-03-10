<template>
  <div class="movie-reuslts border border-danger">
      <h3>Search Results:</h3>
      <ol>
          <li v-for="movieData in state.movies" :key="movieData.id">
              <Movie :movies="movieData"/>

          </li>
      </ol>
  </div>
</template>

<script>
import { reactive } from '@vue/reactivity'
import { computed } from 'vue'
import { AppState } from '../AppState'
import Movie from './Movie'

export default {
  name: 'MovieResults',
  setup () {
    const state = reactive({
      movies: computed(() => AppState.movies)
    })
    return state
  }
    components: {
        Movie
    }
}
</script>

<style scoped>
li{
cursor: pointer;
}
li:hover{
    background-color: #add8e6;
}

</style>
