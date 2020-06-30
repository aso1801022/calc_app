<template>
  <div id="app">
   <Calc  v-bind:title="message"
   v-on:result-event="appAction"/>
   <hr>
   <div><table v-html="log"></table></div>
  </div>
</template>

<script>

import Calc from './components/Calc.vue'

export default {
  name: 'App',
  components: {
    Calc
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
