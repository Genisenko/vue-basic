<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <NavBar/>
    <FooterPage/>
    <MaTh></MaTh>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import NavBar from './components/navBar.vue';
import FooterPage from './components/footerPage.vue';
import MaTh from './components/MaTh.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    NavBar,
    FooterPage,
    MaTh
}
}
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
