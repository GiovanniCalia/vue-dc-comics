<template>
  <div id="app">
    <DCcomics />
    <jumbotronMain />
    <mainDCcomics />
    <footerDCcomics />
  </div>
</template>

<script>
import DCcomics from './components/DCcomics.vue'
import jumbotronMain from './components/jumbotronMain.vue'
import mainDCcomics from './components/mainDCcomics.vue'
import footerDCcomics from './components/footerDCcomics.vue'

export default {
  name: 'App',
  components: {
    DCcomics,
    jumbotronMain,
    mainDCcomics,
    footerDCcomics
  }
}
</script>

<style lang="scss">
@import './assets/styles/stile.css';
</style>
