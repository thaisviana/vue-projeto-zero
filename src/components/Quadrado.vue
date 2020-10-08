<template>
  <div class="box"> 
    <div> <p>Quadrado:</p></div>
    <div> <h3>{{ numero ** 2 }}</h3></div>
  </div>
</template>

<script>
export default {
  name: 'Quadrado',
  props: {
    numero: Number,
    mensagem: String,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
