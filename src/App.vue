<script>
import AppMain from './components/AppMain.vue';
import AppHeader from './components/AppHeader.vue';

import {store} from './store.js';
import axios from "axios";

export default {
  data() {
    return {
      store,
    }
  },
  components: {
    AppMain,
    AppHeader,
  },
  created(){
    axios.get("https://api.themoviedb.org/3/search/movie?api_key=86b5d08d37b03ee809239f83c7709f1c&query=kung%20fu%20panda").then((response)=>{
      console.log(response);
    });
  },
}
</script>

<template>

  <AppHeader></AppHeader>

  <AppMain></AppMain>
  
</template>

<style scoped>

</style>
