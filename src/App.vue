<template>
  <div>
    <MainComponent/>
    <LifeCycle/>  
    <Pessoa/>  
  </div> 
</template>

<script>
import MainComponent from './components/MainComponent.vue';
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue';

  export default {
    name: "App",
    components: { MainComponent, LifeCycle, Pessoa }
}
</script>

