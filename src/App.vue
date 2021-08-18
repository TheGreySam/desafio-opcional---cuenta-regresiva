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
  <cuenta-regr></cuenta-regr>
    <CuentaRegr></CuentaRegr>
 
  <div>
    <button class="btn btn-danger" style="width: 25%;" @click="iniciarCuenta"><h3>Iniciar!</h3></button>
  </div>
</div>
  </div>
</template>

<script>

//export default {
//  name: 'App',
//  el: "",
//  data: () => ({
//    nuevaCuenta: "OJO",
//    textoCuenta: ["Aquí iniciará la cuenta regresiva"],
//  }),
//  methods: {
//    agregar5segundos() {
//      this.textoCuenta.push(this.nuevaCuenta)
//      this.nuevaCuenta = "cuenta regresiva";
//    },
//  },

import CuentaRegr from "./components/CuentaRegr.vue";
import CuentaRegr from "./components/CuentaRegr.vue";

//    name: 'CuentaRegresiva',
//    data () {
//      return {
 //       horas: 0,
//        minutos: 0,
//        segundos: 0,
//      }
//    },
//    mounted(){
//    setInterval(this.actualizarCuenta,1000)
//    },
//    methods: {
//      updateCounter() {
//        let now = new Fecha();
//        let end = new Fecha(this.fechaEnd);
//        let distancia = end - now;
//        if(distancia > 0) {
//          this.horas = Math.floor((distancia % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
//          this.minutos = Math.floor((distancia % (1000 * 60 * 60)) / (1000 * 60));
//          this.segundos = Math.floor((distancia % (1000 * 60)) / 1000);
//        }else{
//          this.horas = 0;
//          this.minutos = 0;
//          this.segundos = 0;
//        }
//      }
//
//    }
//
//}


</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -we
  components: { CuentaRegr },bkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: g
  components: { CuentaRegr },rayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

</style>
