<template>
  <div id="app">
    <input type="text" v-model="clienteVictor.nome"><br>
    <input type="text" v-model="clienteVictor.email">
    <Cliente :cliente="clienteVictor" :showAge="true"/>
    <Cliente :cliente="clienteVictor" :showAge="false"/>
    <Cliente :cliente="clienteVictor" :showAge="true"/>
  </div>
</template>

<script>
import Cliente from "./components/Cliente"
// import Produto from "./components/Produto"

export default {
  name: 'App',
  data(){
    return {
      clienteVictor: {
        nome: "Victor Lima",
        email: "victor@gmail.com",
        idade: 33,
      }
    }
  },
  components: {
    Cliente,
    // Produto
  }

}
</script>

<style>

</style>
