<template>
  <div>
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

  export default {
    name: "App",
    components: { MainComponent, LifeCycle, Pessoa, Form }
}
</script>

<style scoped>
  body {
    background-color: #333;
    color: #FFF;
  }
</style>

