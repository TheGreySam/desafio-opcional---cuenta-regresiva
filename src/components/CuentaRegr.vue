<template>
    <ul>
    <li>horas: {{ hours }}</li>
    <li>minutos: {{ minutes }}</li>
    <li>segundos: {{ seconds }}</li>
  </ul>
</template>

<script>
import moment from "moment";

export default {
  name: "CuentaRegresiva",
  data: () => ({
    time: moment(),
    interval: null,
  }),
  mounted() {
    this.interval = setInterval(() => {
      this.time = moment();
    }, 1000);
  },
  destroyed() {
    window.clearInterval(this.interval);
  },
  computed: {
    hours() {
      return this.time.format("HH");
    },
    minutes() {
      return this.time.format("mm");
    },
    seconds() {
      return this.time.format("ss");
    },
  },
};
</script>

<style scoped>

</style>