<template>
  <div id="app">
    <Heder msg="Mundo"/>
    <HelloWorld msg="World"/>
    <img alt="Vue logo" src="./assets/logo.png">
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Heder from './components/Heder.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Heder
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
