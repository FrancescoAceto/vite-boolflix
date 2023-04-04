<script>
import {store} from '../store.js';

export default {
    name: "AppMain",
  data() {
    return {
        store,
    }
  },
}
</script>

<template>
  <h1>BOOLFLIX</h1>

  <div v-for="movie in store.movies">
      {{ movie.title }}
  </div>

</template>

<style scoped>

h1{
  color: red;
  font-size: 70px;
  text-align: center;
}
</style>