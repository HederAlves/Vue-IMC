<template>
    <section>
          <div class="blocoPrincipal">
            <div class="blocoInput">
            <button class="novoTeste" onclick="window.location.reload();">Novo Teste</button>
                <ul>
                    <li>
                    <h2>Altura (ex.:1,70)</h2>
                      <input class="altura" v-model="input_altura" type="number">
                    </li>
                    <li>
                      <h2>Peso (ex.:69,20)</h2>
                      <input class="peso" v-model="input_peso" type="number">
                    </li>
                </ul>
                  <input class="botaoResultado" type="submit" value="Resultado" v-on:click="calculaIMC">
                  <p class="resultadoImc">{{ resultado }}</p>
            </div>
          </div>
    </section>
</template>

<script>
  
export default {
  name: 'SectionUser',
  data () {
      
    return {
      input_altura: "",
      input_peso: "",
      resultado: ""
    }
  },
  methods: {
    
    calculaIMC(e) {

      var altura = Number(this.input_altura)
      var peso = Number(this.input_peso)
      var resultado = peso / (altura * altura)

      e.preventDefault();
      this.resultado = resultado.toFixed(2);
      //emitir um evento e passar o resultado como parâmetro.
      this.filtro(resultado)

    }
  }
}

</script>

<style scoped>
  .blocoPrincipal {
    position: absolute;
    margin: -510px 0px 0px 925px;
    width: 220px;
    height: 400px;
    box-sizing: border-box;
    border-radius: 15px;
    padding: 8px 15px;
    align-items: right;
    color: hsl(255,95%,95%);
}

.novoTeste {
    margin: 15px 0px 0px 20px;
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

.blocoInput {
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    height: 630px;
    border-radius: 15px;
    background: black;
    margin-top: 150px;
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
    margin: 22px;
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
    padding: 50px 10px 50px 10px;
    background: hsl(255,95%,95%);
    border-radius: 15px;
    margin: 20px;
}
</style>