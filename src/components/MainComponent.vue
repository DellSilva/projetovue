<template>
    <div>
        <h1>Olá vue!</h1>
        <h2>agora sim !!!!!</h2>
        <p>Meu nome é {{ nome }} e sou um {{ profissao }} </p>
        <MultiplosEventos />
        <Reutiliza/>
    </div>

</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue';
import Reutiliza from './Reutiliza.vue';
export default {
    name: "MainComponent",
    data() {
        return {
            nome: "Dell Silva",
            profissao: "dev junior"
        };
    },
    components: { MultiplosEventos, Reutiliza }
}
</script>