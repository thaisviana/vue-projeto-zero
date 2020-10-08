<template>
  <div class="box"> 
        <div> <p>Cubo:</p></div>
        <div> <h3>{{ numero ** 3 }}</h3></div>
    </div>
</template>

<script>
export default {
  name: 'Cubo',
  props: {
    numero: Number
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
