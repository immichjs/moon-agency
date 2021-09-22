<template>
  <div id="app">
    <Header />
  </div>
</template>

<script lang="ts">
import Vue from 'vue';

import Header from '@/components/Header.vue'

export default Vue.extend({
  name: 'App',
  components: {
    Header
  }
});
</script>

<style lang="sass">
@import './assets/sass/base/index'
</style>
