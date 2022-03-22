<template>
  <div id="app">
    <DCcomics />
    <mainDCcomics />
    <footerDCcomics />
  </div>
</template>

<script>
import DCcomics from './components/DCcomics.vue'
import mainDCcomics from './components/mainDCcomics.vue'
import footerDCcomics from './components/footerDCcomics.vue'

export default {
  name: 'App',
  components: {
    DCcomics,
    mainDCcomics,
    footerDCcomics
  }
}
</script>

<style lang="scss">
@import './assets/styles/stile.css';
</style>
