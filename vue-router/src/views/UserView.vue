<template>
    <h1>Seu nome é {{ nome }} e isso é um teste!</h1>
    <p>Teste bem sucedido!</p>
    <input type='text' name='Email' id='email' placeholder='exemplo@exemplo.com.br'><br>
    <input type='text' name='Senha' id='senha' placeholder='Exemplo@123'><br>
    <button>Enviar</button>
    <h4>{{ routeParameter }}</h4>
    <router-view/>
</template>

<script>
export default{
    created(){
        //this.routeParameter = this.$route.params.id;
    },
    data(){
        return{
            nome:'Ezequiel',
            routeParameter: 'Nada'
        }   
    }
}
</script>