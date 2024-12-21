<template>
<ClienteTeste/>
<ClienteTeste/>
<!-- Os componentes podem ser repetidos inumeras vezes... são reeaproveitaáveis -->
<PrecoTeste/>
<PrecoTeste/>
</template>

<script>
import ClienteTeste from './components/Cliente.vue'
import PrecoTeste from './components/Preco.vue'

export default {
  name: 'App',
  components: {
    ClienteTeste,
    PrecoTeste,
  }
}
</script>

<style>
</style>
