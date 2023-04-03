<script>
import AppMain from './components/AppMain.vue';
import AppHeader from './components/AppHeader.vue';

import {store} from './store.js';

export default {
  data() {
    return {
      store,
    }
  },
  components: {
    AppMain,
    AppHeader,
  }
}
</script>

<template>

  <AppHeader></AppHeader>

  <AppMain></AppMain>
  
</template>

<style scoped>

</style>
