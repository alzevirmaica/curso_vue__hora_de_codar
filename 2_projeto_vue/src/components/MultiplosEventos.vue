<template>
  <div>
    <button @click="Primeiro(txt1, $event), Segundo(txt2, $event), Terceiro()">Ativar múltiplos eventos</button>
    <p>{{ multiplos_eventos }}</p>
  </div>
</template>

<script>
export default {
 name: 'MultiplosEventos',
 data() {
    return {
        multiplos_eventos: "",
        txt1: "Primeiro evento ativado!",
        txt2: "Segundo evento"
    }
 },
 methods: {
    Primeiro(txt,e) {
        this.multiplos_eventos = txt
    },
    Segundo(txt,e) {
        setTimeout(() => this.multiplos_eventos = txt, 500)
    },
    Terceiro() {
        setTimeout(() => this.multiplos_eventos = "", 1500)
    }
 },
}
</script>

<style scoped>
    div {
        margin: 100px;
    }
</style>