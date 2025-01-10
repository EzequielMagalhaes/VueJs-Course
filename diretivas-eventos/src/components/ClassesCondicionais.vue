<template>
    <div :class="{'condicional': !isPremium, 'condAdicional': isPremium}">
        <h4>Nome : {{ cliente.nome }}</h4><hr>
        <p>Email: {{ cliente.email }}</p>
        <p v-if='mostrarIdade == true'>Idade: {{ cliente.idade }}</p>
        <p v-else>O usuário escondeu sua idade.</p>
        <p v-show='mostrarIdade === true'>Idade: {{ cliente.idade }} - Método show</p>      
    </div>
</template>

<script>
export default {
    name:'ClassesCondicionaisTeste',
    data(){
        return {
            isPremium: false
        }
    },
    props:{
        cliente: Object,
        mostrarIdade: Boolean
    }
}
</script>

<style scoped>
    .condicional{
        background-color: grey;
        padding: 2%;
        margin-top: 2%;
    }
    .condAdicional{
        background-color: black;
        color: yellow;
        padding: 2%;
        margin-top: 2%;
    }
</style>