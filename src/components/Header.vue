<template>
    <header>
        <h1>Calcula IMC</h1>
        <div class="blocoCabecalho">
            <p class="paragrafoCabecalho">IMC é a sigla para Índice de Massa Corpórea, parâmetro adotado pela Organização Mundial de Saúde para calcular o peso ideal de cada pessoa.</p>
            <p class="paragrafoCabecalho">O índice é calculado da seguinte maneira: divide-se o peso do paciente pela sua altura elevada ao quadrado. Diz-se que o indivíduo tem peso normal quando o resultado do IMC está entre 18,5 e 24,9.</p>
            <p class="paragrafoCabecalho"> Quer descobrir seu IMC? Insira seu peso e sua altura nos campos e compare com os índices da tabela. Importante: siga os exemplos e use pontos como separadores.</p>
        </div>
    </header>    
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style scoped>
    header {
    width: 80%;
    height: 560px;
    background: black;
    padding: 20px;
    box-sizing: border-box;
    border-radius: 15px;
    margin-left: 130px;
}

h1 {
    text-align: center;
    position: absolute;
    margin-top: -55px;
    font-weight: bold;
    font-size: 35px;
    color: hsl(255,60%,60%);
    font-family: sans-serif;
    font-weight: bold;
    box-sizing: border-box;
    width: 30%;
    padding: 20px 0px 0px 0px;
    line-height: 1.5;
    background: hsl(255,95%,95%);
    border-radius: 15px;
    height: 90px;
}

.blocoCabecalho {
    display: flex;
    color: hsl(255,95%,95%);
    font-family: sans-serif;
    font-style: italic;
    box-sizing: border-box;
    width: 65%;
    padding: 20px;
    line-height: 1.5;
    background: hsl(255,60%,60%);
    margin-top: 60px;
}

.paragrafoCabecalho {
    margin: 0px 25px 0px 0px;
}
</style>