<template>
  <div id="app">
    <div> <h1>{{ numero }}</h1></div>
    <div class="result">
      <quadrado :numero="numero" :mensagem="mensagem" />
      <cubo :numero="numero" />
      <raiz :numero="numero" />
      <fatorial :numero="numero" />
      <primo :numero="numero" />
      <ParOuImpar :numero="numero" />
      
    </div>
  </div>
</template>

<script>
import Quadrado from './components/Quadrado.vue'
import Cubo from './components/Cubo.vue'
import Raiz from './components/Raiz.vue'
import Fatorial from './components/Fatorial.vue'
import Primo from './components/Primo.vue'
import ParOuImpar from './components/ParOuImpar.vue'

export default {
  name: 'App',
  data(){
    return {
      numero : 5,
      mensagem : "OI",
    }
  },components: {
    Quadrado,
    Fatorial,
    Cubo,
    Raiz,
    ParOuImpar,
    Primo,
  }
}
</script>

<style>
.result{
  display : flex;
  width: 90%;
  margin: 0 auto;
  flex-wrap: wrap;
}
body{
  padding : 20px;
}
p{
  font-size: 24px;
}
#app{
  text-align: center;
}
.box{
  width: 27%;
  border: black 1px solid;
  padding: 5px;
  margin: 10px;
  text-align: center;
}
</style>
