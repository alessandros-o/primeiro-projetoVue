<template>
    <div class="contador">
        <h2>Contador: {{ contador }}</h2>
        <button @click="subtrair">-</button>
        <button @click="somar">+</button>
    </div>    
</template>

<script>
export default {
    name: 'ContadorGeral',
    data(){
        return{
            contador: 0
        }
    },
    methods:{
        somar(){
            this.contador = this.contador + 1;
        },
        subtrair(){
            this.contador = this.contador - 1;
        }
    }
}
</script>

<style scoped>

</style>