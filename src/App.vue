<template>
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->

  <h1>Watcher</h1>
  <WatcherComponent />
  <hr />
  <h1>Computed Properties</h1>
  <ComputedProperties />
  <hr />
  <h1>BindingClass</h1>
  <BindingClass />
  <hr />
  <h1>BindingStyle</h1>
  <BindingStyle />
  <hr />
  <h1>ConditionalRendering</h1>
  <ConditionalRendering />
  <hr />
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import WatcherComponent from "./components/WatcherComponent.vue";
import ComputedProperties from "./components/ComputedProperties.vue";
import BindingClass from "./components/BindingClass.vue";
import BindingStyle from "./components/BindingStyle.vue";
import ConditionalRendering from "./components/ConditionalRendering.vue";
export default {
  name: "App",
  components: {
    // HelloWorld,
    WatcherComponent,
    ComputedProperties,
    BindingClass,
    BindingStyle,
    ConditionalRendering,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
