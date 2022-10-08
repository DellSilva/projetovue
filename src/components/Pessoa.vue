<template>
    <div>
        <h2>Meu nome é {{ nome }}</h2> 
        <Info :email="email"/>
    </div>
</template>

<script>
    import Info from './Info.vue';

    

    export default {
        name: 'Pessoa',
        components: {
            Info
    },
        data() {
            return {
                nome: 'Dell',
                email: 'adelmo.dev@gmail.com'
            }
        }
    }
</script>