<template>
    <div id='props'>
        <h4>Nome : {{ nome }}</h4><hr>
        <p>Email: {{ email }}</p>
        <p>Idade: {{ idade }}</p><br><hr><hr>
<!-- Usando o Object -->
        <h4>Nome : {{ cliente.nome }}</h4><hr>
        <p>Email: {{ cliente.email }}</p>
        <p>Idade: {{ cliente.idade }}</p>
    </div>

</template>

<script>
export default {
    name:'PropsTeste',
    data(){
        return {
            //nome: 'Ezequiel', // Se deixar aqui, vai causar erro por duplicade com a props instanciada abaixo. 
            //email: 'exemlo@exemplo.com.br',
            //idade: 0
        }
    },
    props:{
        nome: String, //O atributo tem que ser algum tipo Javascript (String, Number, Array, Object,etc) 
        email: String,
        idade: Number,
        cliente: Object
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