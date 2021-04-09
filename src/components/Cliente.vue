<template>
    
    <div id="cliente">
        <input type="text" :value="nome">
        <hr>
        <input type="text" :value="descrição">
        <h2 id="cliente-nome">{{ nome }}</h2>
        <p> descrição do cliente: {{ descrição }} </p>
        
    </div>
    
</template>

<script>
export default {
    data(){
        return {
            nome: "Alisson Andrade",
            numero: "",
            email: "",
            idade: 0,
            descrição: "Lorem Ipsun Lorem Ipsun"
        }
    }
}
</script>

<style scoped>
    #cliente{
        color:blue;
    }

</style>