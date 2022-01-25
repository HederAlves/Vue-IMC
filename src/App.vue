<template>
  <div id="app">
    <h1>{{ titulo }}</h1>
    <Header/>
    <Tabela/>
    <SectionUser/>
  </div>
</template>

<script>

import Header from './components/Header.vue'
import Tabela from './components/Tabela.vue'
import SectionUser from './components/SectionUser.vue'

export default {
  name: 'App',
  components: {
    Header,
    Tabela,
    SectionUser,
  }
}
</script>

<style scoped>
  #app {
    margin: 0 auto;
    background: hsl(255,60%,60%);
    padding: 60px 0px 0px 0px;
    height: 607px;
}
</style>
