<template>
    <div>
        <h1>Olá Vue!</h1>
        <p>Meu nome é {{ nome }}, e a minha profissão é {{ profissao }}</p>
    </div>
</template>

<script>
  export default {
    name: 'PrimeiroComponente',
      data() {
        return {
          nome: "Alzevir",
          profissao: "Programador"
        }
      }
    }
</script>