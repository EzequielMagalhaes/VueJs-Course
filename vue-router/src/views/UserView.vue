<template>
    <h1>Seu nome é {{ nome }} e isso é um teste!</h1>
    <p>Teste bem sucedido!</p>
    <input type='text' name='Email' id='email' placeholder='exemplo@exemplo.com.br'><br>
    <input type='text' name='Senha' id='senha' placeholder='Exemplo@123'><br>
    <input type='submit' name='Enviar' id='enviar'>
</template>

<script>
export default{
    data(){
        return{
            nome:'Ezequiel'
        }   
    }
}
</script>