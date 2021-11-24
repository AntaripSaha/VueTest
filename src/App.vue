<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <Google />
    <Home />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Google from "./components/GoogleTrans.vue";
import Home from "./components/Home.vue";
export default {
  name: "App",
  components: {
    Google,
    Home,
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
