<template>
    <div>             
        <p v-if="esta_trabalhando">Estou estudando no momento</p>
        <p v-else>Utilizo as seguintes tecnologia:</p>
        <ul>
            <li>JavaScript</li>
            <li>Vue</li>
            <li>PHP</li>
            <li>Laravel</li>
        </ul>
        <div>
            <button @click="showEmail">{{ textoBotao }}</button>
        </div>
        <p v-show="mostrar_email">mande mensagem para: {{email}}</p>
        <p>click <a v-bind:href="link" target="_blank">aqui</a> para acessar o portifólio</p>
        <Picture/>
    </div>
</template>

<script>
import Picture from './Picture.vue';
    export default {
    name: "Info",
    data() {
        return {
            esta_trabalhando: false,
            mostrar_email: false,
            email: "adelmo.dev@gmail.com",
            link: "https://www.google.com.br/",
            textoBotao: 'Mostrar e-mail'
        };
    },
    methods: {
        showEmail() {
            this.mostrar_email = !this.mostrar_email
            if(!this.mostrar_email) {
                this.textoBotao = 'Mostrar e-mail'
            } else {
                this.textoBotao = 'Ocultar e-mail'
            }
        }
    },
    components: { Picture }
}
</script>