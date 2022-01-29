<template>
  <div id="app">
    <h1>{{ titulo }}</h1>
    <Header/>
    <Tabela :list="listaDeTarefas" />
  <button @click="filtro(resultado)">iuyegueydgeyh</button>
     <!-- evento.SectionUser<button @click='filtro'>Teste</button>-->
    <SectionUser/>
    <!-- pegar o evento SectionUser e disparar uma função(filtro) parâmetro resultado. -->
  </div>
</template>

<script>

import Header from './components/Header.vue'
import Tabela from './components/Tabela.vue'
import SectionUser from './components/SectionUser.vue'

const list = [
  {
   imc: "Menor que 18,5",
   classificacao: "Magreza",
   obesidade: "0"    
  },
  {
   imc: "Entre 18,5 e 24,9",
   classificacao: "Normal",
   obesidade: "0"
  },
  {
   imc: "Entre 25,0 e 29,9",
   classificacao: "Sobrepeso",
   obesidade: "1"    
  },
  {
   imc: "Entre 30,0 e 39,9",
   classificacao: "Obesidade",
   obesidade: "2"    
  },
  {
   imc: "Maior que 40,0",
   classificacao: "Obesidade Grave",
   obesidade: "3"    
  }
]

export default {
  name: 'App',
  components: {
    Header,
    Tabela,
    SectionUser
  },

  data () {
    
    return{
      listaDeTarefas: list
    }
  },
  methods: {
    //resultado
    filtro() {
      const novaLista = this.listaDeTarefas.filter((tarefa) => {
         if (tarefa.obesidade == 0) {
            return true
         } else {
           return false
         }
       })
      this.listaDeTarefas = novaLista
    }
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
