<template>
    <div>
        <h1>Olá vue!</h1>
        <h2>agora sim !!!!!</h2>
        <p>Meu nome é {{ nome }} e sou um {{ profissao }} </p>
    </div>

</template>

<script>
    export default {
        name: 'MainComponent',
        data() {
            return {
                nome: "Dell Silva",
                profissao: "dev junior"
            }
        }
    }
</script>