<template>
    <div id='props'>
        <h4>Nome : {{ nome }}</h4><hr>
        <p>Descrição: {{ descricao }}</p><hr>
        <p>Número: {{ numero }}</p>
        <p>Email: {{ email }}</p>
        <p>Idade: {{ idade }}</p>
    </div>

</template>

<script>
export default {
    name:'PropsTeste',
    data(){
        return {
            //nome: 'Ezequiel', // Se deixar aqui, vai causar erro por duplicade com a props instanciada abaixo. 
            descricao: 'Descrição de teste',
            numero:'(xx) x xxxx-xxxx',
            //email: 'exemlo@exemplo.com.br',
            //idade: 0
        }
    },
    props:{
        nome: String, //O atributo tem que ser algum tipo Javascript (String, Number, Array, Object,etc) 
        email: String,
        idade: Number
    }
}
</script>

<style scoped>
    #props{
        background-color: grey;
        padding: 2%;
        margin-top: 2%;
    }
</style>