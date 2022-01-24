<template>
    <div>
        <h1>Seu Imc é </h1>
        <h1>{{ oi }}</h1>
        <h1>{{ m }}</h1>
    </div>
  

</template>

<script>
var nome = prompt('Olá, qual é seu nome')
var peso = prompt('Por favor digite seu peso')
var altura = prompt('Por favor digite sua altura')
var resultadoIMC = parseFloat ( peso )  /  ( parseFloat ( altura )  *  parseFloat ( altura ) ) 

export default {
    name: 'IMC',
    data () {
        return {
            oi: resultadoIMC,
            m: nome
        }
    }
}

</script>