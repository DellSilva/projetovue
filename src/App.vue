<template>
  <div>
    <Header :esta_logado = "true"/>
    <MainComponent/>
    <LifeCycle/>  
    <Pessoa/>  
    <Form/>
  </div> 
</template>

<script>
import MainComponent from './components/MainComponent.vue';
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue';
import Form from './components/Form.vue';
import Header from './components/Header.vue';

  export default {
    name: "App",
    components: { MainComponent, LifeCycle, Pessoa, Form, Header }
}
</script>

<style scoped>
  body {
    background-color: #333;
    color: #FFF;
  }
</style>

