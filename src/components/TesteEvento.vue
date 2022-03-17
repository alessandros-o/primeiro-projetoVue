<template>
    <div class="teste-evento">
        <h1>Teste Evento</h1>
        <p v-if="valida" @click="deixarMaiuscula">{{ mensagem }}</p>
        <p v-else @click="deixarMinuscula">{{ mensagem }}</p>
    </div>
</template>

<script>
export default {
    name: 'TesteEvento',
    data(){
        return{
            mensagem: 'Qualquer mensagem',
            valida: true
        }
    },
    methods:{
        deixarMaiuscula(){
            this.mensagem = this.mensagem.toUpperCase();
            this.valida = false;
        },
        deixarMinuscula(){
            this.mensagem = this.mensagem.toLowerCase();
            this.valida = true;
        }
    }
    
}
</script>

<style scoped>

</style>