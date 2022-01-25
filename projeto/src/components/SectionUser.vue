<template>
    <section>
          <div>
            <div>
                <button onclick="window.location.reload();">Novo Teste</button>
                <ul>
                    <li>
                    <h2>Altura (ex.:1,70)</h2>
                      <input v-model="altura" type="number">
                      {{ altura }}
                    </li>
                    <li>
                      <h2>Peso (ex.:69,20)</h2>
                      {{ peso }}
                      <input v-model="peso" type="number">
                    </li>
                </ul>
                <button v-on:click="CalculaIMC()">Resultado</button>
                <p v-bind="resutadoIMC"></p>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data () {
      return {
        peso: "",
        altura: "",
      }
    }
}
</script>