<template>
  <h1>Conversor de Moedas</h1>

  <div class="linha">
    <Conversor class="card" moeda-a="USD" moeda-b="BRL" />
    <Conversor class="card" moeda-a="BRL" moeda-b="USD" />
  </div>

  <div class="linha">
    <Conversor class="card" moeda-a="CAD" moeda-b="BRL" />
    <Conversor class="card" moeda-a="BRL" moeda-b="CAD" />
  </div>

  <div class="linha">
    <Conversor class="card" moeda-a="EUR" moeda-b="BRL" />
    <Conversor class="card" moeda-a="BRL" moeda-b="EUR" />
  </div>
</template>

<script>
import Conversor from "./components/Conversor.vue";

export default {
  name: "App",
  components: {
    Conversor,
  },
};
</script>

<style>
#app {
  margin: auto;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.card{
  border-radius: 5px;
}

.linha{
  display: flex;
  justify-content: space-around;
  margin-top: 40px;
}
</style>
