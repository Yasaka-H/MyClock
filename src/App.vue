<template>
  <div id="app">
    This is world clock
    <main-clock></main-clock>
  </div>
</template>

<script>
import mainClock from './components/mainClock.vue'

export default {
  name: 'app',
  components: {
    mainClock
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
