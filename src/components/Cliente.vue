<template>
    
    <div :class="{'cliente': !isPremium, 'cliente-premium': isPremium}">
        <h4>Nome: {{ cliente.nome }} </h4>
        <p>Email: {{ cliente.email }}</p>
        <p v-if="showAge == true">Idade: {{ cliente.idade }}</p>
        <p v-else>Esse usuario não informou a idade</p>
    </div>
    
</template>

<script>
export default {
    data(){
        return {
            isPremium: true
        }  
    },
    props: {

        cliente: Object,
        showAge: Boolean

    }
}
</script>

<style scoped>
    .cliente{
        background-color: #ECE5E3;
        max-width: 600px;
        height: 100px;
        padding: 2%;
        margin-top: 2%;
    }
    .cliente-premium{
        background-color: black;
        color: yellow;
        max-width: 600px;
        height: 100px;
        padding: 2%;
        margin-top: 2%;
    }

</style>