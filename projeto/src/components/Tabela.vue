<template>
    <div>
        <table class="tabela">
            <thead>
                <tr>
                    <th>Imc</th>
                    <th>Classificação</th>
                    <th>Obesidade</th>
                </tr>
            </thead>
            <tbody>
                <tr id="magreza" magreza>
                    <td>Menor que 18,5</td>
                    <td>Magreza</td>
                    <td>0</td>
                </tr>               
                <tr id="normal">
                    <td>Entre 18,5 e 24,9</td>
                    <td>normal</td>
                    <td>0</td>
                </tr>
                <tr id="sobrepeso">
                    <td>Entre 25,0 e 29,9</td>
                    <td>Sobrepeso</td>
                    <td>1</td>
                </tr>
                <tr id="Obesidade">
                    <td>Entre 30,0 e 39,9</td>
                    <td>Obesidade</td>
                    <td>2</td>
                </tr>
                <tr id="obsidadeGrave">
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