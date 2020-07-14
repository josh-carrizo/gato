<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Milista titulo="Actividades realizadas" :actividad="hechos" />
    <Milista titulo="Actividades post-cuarentena" :actividad="por_hacer" />
    <br> <br> <br>
  </div>
</template>

<script>
import Milista from './components/Milista.vue'

export default {
  name: 'App',
  components: {
    Milista
  },
  data: () => {
    return {
      // acá están mis datos
      hechos: [
        "Terminar la U",
        "Viajar",
        "Grabar música",
        "Crear contenido",
        "Emprender"
      ],
    }
  }
}
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