<template>
  <input type="text" v-model="dadosDoCliente.nome">
  <input type="text" v-model="dadosDoCliente.email">
  <PropsTeste :nome="dadosDoCliente.nome" :email='dadosDoCliente.email' :idade='dadosDoCliente.idade'/>
  <PropsTeste nome='Ezequiel Magalhães' email='zekiel.dev@gmail.com' idade='21'/>
  <PropsTeste nome='Nathalia Silvana Tomm de Souza' email='natthytdz@gmail.com' idade='20'/>
  <PropsTeste nome='Testando props' email='teste@teste.com' idade='teste'/>
</template>

<script>
import PropsTeste from './components/Props.vue'
export default {
  name: 'App',
  data(){
    return{
      dadosDoCliente:{
        nome:'Anakin Skywalker',
        email:'anksky@gmail.com',
        idade:'200'
      }
    }
  },
  components: {
    PropsTeste
  }
}
</script>
<style>
</style>
