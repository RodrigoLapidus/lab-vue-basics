<template>
  <div>
    <nav>
      <h1 v-bind:style=" {
        padding: '50px',
        backgroundColor: 'lightgray',
        color: 'white',
      }">This is the navbar</h1>
    </nav>
    
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <MainComponent />
    
    <footer v-bind:style=" {
      padding: '30px',
      backgroundColor: 'lightgrey',
      color: 'white',
    }">
      <h1>This is the footer</h1>
    </footer>

  </div>

</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import MainComponent from "./components/MainComponent.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    MainComponent,
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
