<template>
    <h1>primer componente</h1>
    <section>
        <h3>numero - {{ numero }}</h3>
    </section>
    <button @click="incrementar">+1</button>
    <button @click="descrementar">-1</button>
</template>
<script lang="js" setup>
import {Computed, ref} from 'vue'
const numero = ref(0)
const incrementar = () =>{
    numero.value++
}
const decrementar = () => {
    numero.value--
}
</script>
<style scoped> 
h3 {color: red;}
</style>