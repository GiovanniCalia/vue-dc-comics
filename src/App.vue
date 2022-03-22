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
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}*/
</style>
