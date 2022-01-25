<template>
    <div class="blocoTabela">
            <table class="tabela">
                <thead>
                    <tr>
                        <th>Imc</th>
                        <th>Classificação</th>
                        <th>Obesidade</th>
                    </tr>
                </thead>
                <tbody>
                    <tr data-resultado-magreza>
                        <td>Menor que 18,5</td>
                        <td>Magreza</td>
                        <td>0</td>
                    </tr>               
                    <tr data-resultado-normal>
                        <td>Entre 18,5 e 24,9</td>
                        <td>normal</td>
                        <td>0</td>
                    </tr>
                    <tr data-resultado-Sobrepeso>
                        <td>Entre 25,0 e 29,9</td>
                        <td>Sobrepeso</td>
                        <td>1</td>
                    </tr>
                    <tr data-resultado-obesidade>
                        <td>Entre 30,0 e 39,9</td>
                        <td>Obesidade</td>
                        <td>2</td>
                    </tr>
                    <tr data-resultado-obesidadegrave>
                        <td>Maior que 40,0</td>
                        <td>Obesidade Grave</td>
                        <td>3</td>
                    </tr>
                </tbody>
            </table>
        </div>
</template>

<script>

export default {
    name: 'Tabela'
}
</script>

<style scoped>
table {
    font-family: sans-serif;
    text-align: center;
    width: 50.1%;
    margin: -228px 150px;
}

thead {
    text-transform: uppercase;
    background: hsl(255,95%,95%);
    color: hsl(255,60%,60%);
    font-weight: bold;
}

td {
    text-transform: uppercase;
    background: hsl(255,60%,60%);
    color: hsl(255,95%,95%);
    border: 2px solid #000000;
    padding: 8px 15px;
}

th { 
    text-transform: uppercase;
    border: 2px solid #000000;
    padding: 8px 15px;
}

.blocoPrincipal {
    position: absolute;
    margin: -500px 0px 0px 800px;
    width: 220px;
    height: 400px;
    box-sizing: border-box;
    border-radius: 15px;
    padding: 8px 15px;
    align-items: right;
    color: hsl(255,95%,95%);
}

.blocoInput {
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 610px;
    border-radius: 15px;
    background: black;
}

.novoTeste {
    margin: 0px 17px;
    text-align: center;
    background: hsl(255,60%,60%);
    color:hsl(255,95%,95%);
    font-size: 25px;
    width: 150px;
    height: 50px;
    border-radius: 10px;
    text-align: center;
}

.novoTeste:hover {
    background: hsl(255,95%,95%);
    color:hsl(255,60%,60%);
}

.peso,
.altura {
    text-align: center;
    color: hsl(255,60%,60%);
    font-size: 45px;
    width: 100px;
    height: 50px;
    background: hsl(255,95%,95%);
    border-radius: 5px;
}

li {
    padding: 10px;
}

h2 {
    margin-bottom: 20px;
    color: hsl(255,95%,95%);
    font-size: 25px;
}

.botaoResultado {
    margin: 0px 19px;
    text-align: center;
    background: hsl(255,60%,60%);
    color:hsl(255,95%,95%);
    font-size: 25px;
    width: 150px;
    height: 50px;
    border-radius: 10px;
}

.botaoResultado:hover {
    background: hsl(255,95%,95%);
    color:hsl(255,60%,60%);
}

.resultadoImc {
    align-items: center;
    color: hsl(255,60%,60%);
    font-size: 45px;
    font-weight: bold;
    box-sizing: border-box;
    padding: 100px 10px 100px 10px;
    background: hsl(255,95%,95%);
    border-radius: 15px;
    margin: 15px;
}

</style>