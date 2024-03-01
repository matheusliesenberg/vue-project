<script setup>
import { ref } from 'vue';

const contador = ref(0)
function descrementar(){
  if(contador.value > 0){
    contador.value--;
  }
}
function acrementar(){
  contador.value++;
}
function resetar (){
  contador.value = 0;
}
</script>

<template>
<button @click="acrementar">+</button>
<button @click="descrementar">-</button>
<button @click="resetar">Resetar</button>
<p>valor do contator: {{contador }}</p>
</template>

<style scoped>
button{
  background-color: rgb(255, 0, 0);
  color: rgb(255, 255, 255);
  font-weight: bolder;
  border: 0;
  margin: 2px;
}
</style>
