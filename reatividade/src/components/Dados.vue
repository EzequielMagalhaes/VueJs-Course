<template>
    <input type="text" :value="nome"> <!-- ONE-WAY-DATA BINDING -->
    <br/> <!-- Se houver alteração do lado do navegador, não vai alterar necessariamente o dado passado dentro do value -->   
    <input type="text" :value="descricao"> <!-- Serve apenas para leitura -->
    <hr>
    <h1>Teste de reatividade</h1>
    <p>Meu nome é '{{ nome }}', esse é um exemplo!</p>
    <p>E essa é a '{{descricao}}'</p>
    <hr>
    <input type="text" v-model="nome"> <!-- TWO-WAY-DATA BINDING -->
    <input type="text" v-model="descricao"> <!-- Ao alterar o dado no lado do navegador, qualquer outra exibição desse dado será alterada também em tempo real. -->
</template>

<script>
export default {
    name:"DadosTeste",
    data(){
        return {
            nome: "Ezequiel",
            descricao: "Descrição de teste"
        }
    }
}
</script>

<style scoped>
</style>