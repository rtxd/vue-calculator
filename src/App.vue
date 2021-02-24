<template>
<div class="container">
  <Calculator />
  </div>
</template>

<script>
import Calculator from './components/Calculator.vue'

export default {
  name: 'App',
  components: {
    Calculator
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #a07e0e;
  margin-top: 60px;
  font-size: 32px;
}

.container {
  width: 50vw;
  display: block;
  margin-left: auto;
  margin-right: auto;
}
</style>
