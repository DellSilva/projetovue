<template>
    <div>
        <h1>Meu nome: {{nome}}</h1>
    </div>
</template>

<script>
    export default {
        name: 'LifeCycle',
        data() {
            return {
                nome: 'Ainda não sei'
            }
        },
        created() {
         this.nome = 'Dell'
        },
        mounted() {
         this.nome = 'Dell Silva'
        }
    }
</script>