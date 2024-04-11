<template>
    <div>
        <h2>Esta é a descrição da pessoa: {{ nome }}</h2>
        <Info :email="email" :esta_trabalhando="esta_trabalhando" />
    </div>
</template>

<script>
import Info from './Info.vue'
export default {
 name: 'Pessoa',
 components: {
    Info
 },
 data() {
    return {
        nome: 'Alzevir',
        email: 'alzevirm2@gmail.com',
        esta_trabalhando: false
    }
 }
}
</script>

<style>

</style>