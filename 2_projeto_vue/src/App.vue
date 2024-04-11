<template>
  <div>
    <primeiroComponente />
    <lifeCycle />
    <pessoa />
  </div>
</template>

<script>
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa'
import PrimeiroComponente from './components/PrimeiroComponente.vue'

 export default {
  name: 'App',
  components: {
    PrimeiroComponente,
    LifeCycle,
    Pessoa,
  }
 }
</script>

<style>
body {
  background-color: #333;
  color: #fff;
}

a {
  color: red;
}

.teste {
  background-color: #000;
}
</style>