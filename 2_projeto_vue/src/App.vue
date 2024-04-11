<template>
  <div>
    <primeiroComponente />
    <lifeCycle />
    <pessoa />
    <Form />
  </div>
</template>

<script>
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa'
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import Form from './components/Form.vue'

 export default {
  name: 'App',
  components: {
    PrimeiroComponente,
    LifeCycle,
    Pessoa,
    Form
  }
 }
</script>

<style>

</style>