<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <TestItem data='Please' msg='wait...'/>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import TestItem from './components/TestItem.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld,
   TestItem
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
