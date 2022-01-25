<template>
    <div>
        <h1>{{ IMC }}</h1>
    </div>
</template>

<script>

    const altura = document.querySelector(".altura")
    const peso = document.querySelector(".peso")
    const resultadoIMC = parseFloat(peso) / (parseFloat(altura) * parseFloat(altura));
    

export default {
    
    name: 'CalculaIMC',
    CalculaIMC() {

        return {
            IMC: resultadoIMC
        }
    }
}
</script>