<template>
  <div class="box">
    <div><p>Fatorial:</p></div>
    <div>
      <h3>{{ fatorial() }}</h3>
    </div>
  </div>
</template>

<script>
export default {
  name: "Fatorial",
  props: {
    numero: Number,
  },
  methods: {
    fatorial() {
      let n = this.numero;
      let fatorial = 1;
      for (let i = 1; i <= n; i++) {
        fatorial *= i;
      }
      return fatorial;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
