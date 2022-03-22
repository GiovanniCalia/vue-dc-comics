<template>
  <div id="app">
    <DCcomics />
  </div>
</template>

<script>
import DCcomics from '.components/DCcomics.vue'

export default {
  name: 'App',
  components: {
    DCcomics
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
