<template>
  <div id="app">
    <h1>This is world clock</h1>
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
