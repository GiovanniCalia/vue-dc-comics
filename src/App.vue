<template>
  <div id="app">
    <DCcomics />
    <jumbotronMain />
    <cardsDC />
    <mainDCcomics />
    <footerDCcomics />
  </div>
</template>

<script>
import DCcomics from './components/DCcomics.vue'
import jumbotronMain from './components/jumbotronMain.vue'
import cardsDC from './components/cardsDC.vue'
import mainDCcomics from './components/mainDCcomics.vue'
import footerDCcomics from './components/footerDCcomics.vue'

export default {
  name: 'App',
  components: {
    DCcomics,
    jumbotronMain,
    cardsDC,
    mainDCcomics,
    footerDCcomics
  }
}
</script>

<style lang="scss">
@import './assets/styles/stile.css';
</style>
