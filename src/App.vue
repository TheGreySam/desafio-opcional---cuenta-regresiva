<template>
  <div id="app">
    <h3>Elige la duración de la cuenta regresiva</h3>
    <hr>
    <div>
      <button class="btn btn-primary m-3" @click="agregar5segundos">5 segundos</button>
      <button class="btn btn-primary m-3" @click="agregar10segundos">10 segundos</button>
      <button class="btn btn-primary m-3" @click="agregar15segundos">15 segundos</button>

    </div>
    <div class="card">
  <div 
  id
  class="card-body text-dark" 
  style=""
  v-for="(textoCuenta, $index) in textoCuenta" 
  :key="$index">
    {{ textoCuenta }}
  </div>
  <div>
    <button class="btn btn-danger" style="width: 25%;" @click="iniciarCuenta"><h3>Iniciar!</h3></button>
  </div>
</div>
  </div>
</template>

<script>

export default {
  name: 'App',
  el: "",
  data: () => ({
    nuevaCuenta: "OJO",
    textoCuenta: ["Aquí iniciará la cuenta regresiva"],
  }),
  methods: {
    agregar5segundos() {
      this.textoCuenta.push(this.nuevaCuenta)
      this.nuevaCuenta = "cuenta regresiva";
    },
  },
}
</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

</style>
