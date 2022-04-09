<template>
  <div id="app">
    <h1>Vue JS</h1>
    <Car :power="power" :upPower="upPower" />
  </div>
</template>

<script>
import { ref } from 'vue';
import Car from './components/Car.vue';

export default {
  name: 'App',
  components: {
    Car,
  },
  setup() {
    let power = ref(36);

    const upPower = () => {
      console.log('Aumentar power...');
      power.value++;
    };

    return {
      power,
      upPower,
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
