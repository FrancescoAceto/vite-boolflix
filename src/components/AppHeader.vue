<script>
import {store} from '../store.js';
export default {
    name: "AppHeader",
  data() {
    return {
        store,
    }
  },
}
</script>

<template>
  <div class="searchbar">
    <input v-model="store.searchText" type="text" placeholder="Browse Movies & Series">
    <button>Search</button>
  </div>
</template>

<style scoped>
.searchbar{
  display: flex;
  justify-content: center;
  padding-top: 20px;
  padding-bottom: 20px;
  gap: 10px;

}
</style>