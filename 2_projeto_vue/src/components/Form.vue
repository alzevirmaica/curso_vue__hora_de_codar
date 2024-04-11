<template>
  <div>
    <h2>Meu formulário</h2>
    <form action="" @submit="EnviarFormulario($event)">
        <div>
            <input type="text" v-model="name">
        </div>
        <div>
            <input type="text" v-model="email">
        </div>
         <br>
        <button type="submit">Enviar</button>
    </form>
    <p>Conteúdo</p>
  </div>
</template>

<script>
export default {
    name: 'Form',
    data() {
        return {
            name: '',
            email: ''
        }
    },
    methods: {
        EnviarFormulario(e) {
            e.preventDefault();
            const name = this.name
            const email = this.email


            console.log('Formulário enviado')
            console.log(`O nome é : ${name}`)
            console.log(`O e-mail é : ${email}`)
        }
    },
}
</script>

<style>

</style>