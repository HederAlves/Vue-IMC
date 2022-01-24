<template>
  <div id="app">
    <h1></h1>
    <Heder/>
    <IMC/>
  </div>
</template>

<script>
import Heder from './components/Heder.vue'
import IMC from './components/IMC.vue'

export default {
  name: 'App',
  components: {
    Heder,
    IMC
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
