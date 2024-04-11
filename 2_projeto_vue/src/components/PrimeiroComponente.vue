<template>
    <div>
        <Reutilizacao />
        <h1>Olá Vue!</h1>
        <p>Meu nome é {{ nome }}, e a minha profissão é {{ profissao }}</p>
        <MultiplosEventos />
        <Reutilizacao />
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue'
import Reutilizacao from './Reutilizacao'

  export default {
    components: {
      MultiplosEventos,
      Reutilizacao
    },
    name: 'PrimeiroComponente',
      data() {
        return {
          nome: "Alzevir",
          profissao: "Programador"
        }
      }
    }
</script>