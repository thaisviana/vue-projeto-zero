<template>
  <div class="box"> 
        <div> <p>é Primo:</p></div>
        <div> <h3>{{ isPrime() }}</h3></div>
    </div>
</template>

<script>
export default {
  name: 'Primo',
  props: {
    numero: Number
  }, methods:{
      isPrime() {
      for(var i = 2; i < this.numero; i++)
        if(this.numero % i === 0) return 'Não';
      return 'Sim';
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
