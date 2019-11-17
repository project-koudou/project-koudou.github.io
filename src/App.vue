<template>
  <div id="app">
    <AppBar></AppBar>
    <router-view></router-view>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';

import AppBar from '@/components/AppBar.vue';

export default Vue.extend({
  name: 'app',
  components: {
    AppBar,
  },
});
</script>

<style lang="scss">
@import '../node_modules/bulma/bulma.sass';
</style>
