<template>
  <input type="text" v-model="dadosDoCliente.nome">
  <input type="text" v-model="dadosDoCliente.email">
  <!--
  <PropsTeste :cliente='dadosDoCliente'/>
  <PropsTeste :nome="dadosDoCliente.nome" :email='dadosDoCliente.email' :idade='dadosDoCliente.idade'/>
  <PropsTeste nome='Ezequiel Magalhães' email='zekiel.dev@gmail.com' idade='21'/>
  <CondicionaisTeste :cliente='dadosDoCliente' :mostrarIdade='true'/>
  <CondicionaisTeste :cliente='dadosDoCliente' :mostrarIdade='false'/>

  -->
</template>

<script>
//import PropsTeste from './components/Props.vue'
//import CondicionaisTeste from './components/Condicionais.vue'

export default {
  name: 'App',
  data(){
    return{
      nomeParaTestar:'Anakin Skywalker',
      dadosDoCliente:{
        nome:'Nathália Silvana Tomm de Souza',
        email:'natthytdz@gmail.com',
        idade:'20'
      }
    }
  },
  components: {
    //PropsTeste,
    //CondicionaisTeste
  }
}
</script>
<style>
</style>
