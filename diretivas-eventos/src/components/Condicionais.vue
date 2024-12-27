<template>
    <div id='cond'>
        <h4>Nome : {{ cliente.nome }}</h4><hr>
        <p>Email: {{ cliente.email }}</p>
        <!-- Funciona como um if else, se não passar pela situação true, ele exibe outra função -->
        <p v-if='mostrarIdade == true'>Idade: {{ cliente.idade }}</p>
        <p v-else>O usuário escondeu sua idade.</p>
        <!-- Vai mostrar única e exclusivamente quando passar pela situação true --> 
        <p v-show='mostrarIdade === true'>Idade: {{ cliente.idade }} - Método show</p>
    </div>
<!-- Alguns exemplos de diretivas condicionais do VUE são os atributos: 'v-if', 'v-model','v-else','v-else-if','v-show' -->
</template>

<script>
export default {
    name:'CondicionaisTeste',
    data(){
        return {
        }
    },
    props:{
        cliente: Object,
        mostrarIdade: Boolean
    }
}
</script>

<style scoped>
    #cond{
        background-color: grey;
        padding: 2%;
        margin-top: 2%;
    }
</style>