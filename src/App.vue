<template>
  <div id="app">
    <input v-model="clienteRenan.nome"/>
    <Cliente :cliente="clienteRenan" :showYears="true"/>
    <Cliente :cliente="clienteMika" :showYears="false"/>
    <Cliente :cliente="clienteLuna" :showYears="true"/>
    <Cliente :cliente="clienteMeepo" :showYears="false"/>
  </div>
</template>

<script>
import Cliente from './components/Cliente'
export default {
  name: 'App',
  data(){
    return{
      nomeTeste: "Goku Super Saiajin",
      clienteRenan: {
          nome: "Renan",
          idade: "31",
          email:"teste@gmail.com"
      },
      clienteMika: {
          nome: "Mika",
          idade: "23",
          email:"teste@gmail.com"
      },
      clienteLuna: {
          nome: "Luna",
          idade: "3",
          email:"teste@gmail.com"
      },
      clienteMeepo: {
          nome: "Meepo",
          idade: "1",
          email:"teste@gmail.com"
      }
    }
  },
  components:{
    Cliente
  }
}
</script>

<style>

</style>
