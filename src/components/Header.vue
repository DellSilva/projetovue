<template>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Projetos</a></li>
        <li><a href="#">Contato</a></li>
        <li v-if="esta_logado"><a href="#">Meu Perfil</a></li>
    </ul>
</template>
<script>
export default {
    name: 'Header',
    props: ["esta_logado"]
}
</script>

<style scoped>
    ul {
        list-style: none;
        display: flex;
        background: #111;
    }
    li {
        padding-left: 10px;
        visibility: none;
        color: rgb(246, 248, 250);
    }

</style>