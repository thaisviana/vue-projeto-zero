<template>
  <div class="box"> 
        <div> <p>Par Ou Ímpar:</p></div>
        <div> <h3>{{ parOuImpar() }}</h3></div>
    </div>
</template>

<script>
export default {
  name: 'ParOuImpar',
  props: {
    numero: Number
  },
  methods:{
    parOuImpar(){
      return (this.numero % 2 == 0) ? 'Par' : 'Impar';
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
