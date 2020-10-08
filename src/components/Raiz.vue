<template>
  <div class="box"> 
        <div> <p>Raiz:</p></div>
        <div> <h3>{{ Math.sqrt(numero).toFixed(2) }}</h3></div>
    </div>
</template>

<script>
export default {
  name: 'Raiz',
  props: {
    numero: Number
  }
}
</script>
