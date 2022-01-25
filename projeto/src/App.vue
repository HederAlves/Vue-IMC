<template>
  <div id="app">
    <h1>{{ titulo }}</h1>
    <Header/>
    <Tabela/>
    <CalculaIMC/>
    <SectionUser/>
  </div>
</template>

<script>

import CalculaIMC from './components/CalculaIMC.vue'
import Header from './components/Header.vue'
import Tabela from './components/Tabela.vue'
import SectionUser from './components/SectionUser.vue'

export default {
  name: 'App',
  components: {
    CalculaIMC,
    Header,
    Tabela,
    SectionUser,
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
