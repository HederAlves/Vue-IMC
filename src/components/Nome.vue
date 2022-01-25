<template>
    <div>
        <input type="text" v-model="nome">
         {{ nome }}
    </div>
</template>

<script>
export default {

    data () {
      return {
        nome:""
      }
    }
}
</script>