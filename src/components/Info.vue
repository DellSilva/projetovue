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
        <p v-show="mostrar_email">mande mensagem para: {{email}}</p>
    </div>
</template>

<script>
    export default {
        name: 'Info',
        data(){
            return {
                esta_trabalhando: false,
                mostrar_email: true,
                email: 'adelmo.dev@gmail.com'
            }
        }
    }
</script>