<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Estou em busca de novas oportunidades!</p>
        <p>Utilizo as seguintes tecnologias para back-end:</p>
        <ul>
            <li v-bind:key="index" v-for="(technology, index) in backend_technologies">{{ technology }}</li>
        </ul>
        <p>Utilizo as seguintes tecnologias para front-end:</p>
        <ul>
            <li v-bind:key="index" v-for="(technology, index) in frontend_technologies">{{ technology }}</li>
        </ul>
        <div>
            <button @click="showEmail">{{ textoBotao }}</button>
        </div>
        <p v-show="mostrar_email">Mande uma mensagem para: matheus@email.com</p>
        <p>Para acessar meu portfólio <a v-bind:href="link">basta clicar aqui</a></p>
        <Picture />
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
            textoBotao: 'Mostrar e-mail',
            backend_technologies: ["JavaScript", "PHP", "Python"],
            frontend_technologies: ["HTML", "CSS", "Vue"]
        };
    },
    methods: {
        showEmail() {
            this.mostrar_email = !this.mostrar_email
            if (!this.mostrar_email) {
                this.textoBotao = 'Mostrar e-mail'
            } else {
                this.textoBotao = 'Ocultar e-mail'
            }
        }
    },
    components: { Picture }
}
</script>