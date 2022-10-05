<template>
    <div>
        <h2>Meu formulário:</h2>
        <form action="" @submit="enviarFormulario($event)">
            <div>
                <input type="text" v-model="name">
            </div>
            <div>
                <input type="text" v-model="email">
            </div>
            <input type="submit" value="Enviar">
        </form>
    </div>
</template>

<script>
    export default {
        name: 'Form',
        data() {
            return {
                name: "",
                email: ""
            }
        },
        methods: {
            enviarFormulario(e) {

                e.preventDefault();
                const name = this.name;
                const email = this.email;
                console.log('enviado');
                console.log(`o nome é ` + name);
                console.log(`o e-mail é ` + email);
            }
        }
    }
    
</script>