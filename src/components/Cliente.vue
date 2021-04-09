<template>
    
    <div id="cliente">
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