<script setup>
import { ref } from 'vue';
const contador = ref(0)
function descrementar(){
  contador.value--
}
</script>

<template>
<button @click="contador++">+</button>
<button @click="descrementar">-</button>
<p>valor do contator : {{contador }}</p>
</template>

<style scoped></style>
