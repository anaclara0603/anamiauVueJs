<script setup>
import{ref} from 'vue'
  const contador = ref(0);
  function incrementar(){
    contador.value++
  }
  function decrementar(){
    if(contador.value > 0){
      contador.value--
  }}
  function resetar(){
    contador.value = 0
  }
  
</script>

<template>
 <button @click="incrementar">+</button>
 <button @click="decrementar">-</button>
 <button @click="resetar">C</button>
 <p>Valor contador: {{ contador }}</p>
</template>

<style scoped>
  button{
    width: 60px;
    height: 60px;
    background-color: rgb(253, 69, 213);
    color: white;
    font-size: 50px;
    border: none;
    border-radius: 30%;
    margin-left: 20%;
    margin-bottom: 20%;
    
  }
  p{
    font-size: medium;
  }
 body{
  background-image: url("silly ass cats.jpeg");
 }
</style>
