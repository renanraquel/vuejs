<template>
    <div id="cliente">
        <h4>Nome: {{cliente.nome}}</h4>
        <p>Descricao:{{descricao}}</p>
        <p>Telefone:{{telefone}}</p>
        <p>Email:{{cliente.email}}</p>
        <p v-if="showYears === true">Idade:{{cliente.idade}}</p>
        <p v-else>Esse usuário escondeu sua idade</p>
        <p v-show="showYears">Esse usuario Possui idade</p>
    </div>
</template>

<script>
export default {
    data(){
        return{
            telefone: "(43) 98404-6364",
            email:  "renansrr@gmail.com",
            descricao: "Aprendendo Vue.js"
        }
    },
    props:{
        cliente: Object,
        showYears:Boolean
    }
}
</script>

<style scoped>
    #cliente{
        background-color: #ECE5E3;
        color: brown;
        max-width: 600px;
        padding: 1%;
        margin-top: 2%;
    }
    #cliente-premium{
        background-color: black;
        color: yellow;
        max-width: 600px;
        padding: 1%;
        margin-top: 2%;
    }
</style>
