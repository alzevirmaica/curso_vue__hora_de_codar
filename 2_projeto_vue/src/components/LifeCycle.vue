<template>
  <div>
    <h1>Meu nome é: {{ nome }}</h1>
  </div>
</template>

<script>
export default {
    name: 'LyfeCycle',
    data() {
        return {
            nome: 'Ainda não sei'
        }
    },
    created() {
        setTimeout(()=> {
            this.nome = "Alzevir"
        }, 1000)
    },
    mounted() {
        setTimeout(() => {
            this.nome = "Pedro"
        }, 2000) 
    }
}
</script>

<style>

</style>