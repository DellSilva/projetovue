<template>
  <div>
    <MainComponent/>
    <LifeCycle/>    
  </div> 
</template>

<script>
  import MainComponent from './components/MainComponent.vue';
  import LifeCycle from './components/LifeCycle.vue';

  export default {
    name: "App",
    components: [
        MainComponent
    ],
    components: { MainComponent, LifeCycle }
}
</script>

