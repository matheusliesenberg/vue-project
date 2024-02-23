<script setup>
import { ref } from 'vue';

const contador = ref(0)
function descrementar(){
  if(acrementar.value > 0){
    contador.value--
  }
}
function acrementar(){
  contador.value++
}
</script>

<template>
<button @click="acrementar">+</button>
<button @click="descrementar">-</button>
<p>valor do contator: {{contador }}</p>
</template>

<style scoped>
button{
  background-color: chocolate;
  color: white;
  font-weight: bolder;
  border: 0;
  margin: 2px;
}
</style>
