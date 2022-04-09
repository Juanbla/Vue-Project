<template>
  <h2>Coche - Composition API</h2>
  <p>Marca: {{ brand }}</p>
  <p>Modelo: {{ model }}</p>
  <p>Potencia: {{ power }}</p>
  <button @click="upPower">Aumentar</button>
</template>

<script>
export default {
  props: {
    power: {
      type: Number,
      default: 60,
    },
    upPower: Function,
  },
  setup(props) {
    const brand = 'Audi';
    const model = 'A4';
    console.log(props);

    return {
      brand,
      model,

    };
  },
};
</script>

<style scoped>
h2 {
  margin: 40px 0 0;
}

p {
  color: #42b983;
}
</style>
