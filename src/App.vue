<template>
  <div id="app">
    <h3>Elige la duración de la cuenta regresiva</h3>
    <div>
      <button class="btn btn-primary" @click="agregar5segundos">5 segundos</button>
      <button class="btn btn-primary" @click="agregar10segundos">10 segundos</button>
      <button class="btn btn-primary" @click="agregar15segundos">15 segundos</button>

    </div>
    <div class="card">
  <div class="card-body text-dark">
    <h2>cuenta</h2>
  </div>
</div>
  </div>
</template>

<script>

export default {
  name: 'App',
  components: {
    
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
