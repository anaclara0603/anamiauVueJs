<script>
export default {
  data(){
    return{
      contador: 0
    }
  },
  methods:{
    incrementar(){
      this.contador++
    },
    decrementar(){
      if(this.contador > 0){
        this.contador--
      }
    },
    resetar(){
      this.contador = 0
    }
  }
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
    border-radius: 50%;
    margin-left: 20%;
    margin-bottom: 20%;
    
  }
  p{
    font-size: medium;
  }
 
</style>
