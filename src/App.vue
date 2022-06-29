<template>
  <img alt="Vue logo" src="https://upload.wikimedia.org/wikipedia/commons/c/c7/Loading_2.gif" class="center">
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <TestItem class="testitem"/>
  <!-- <TestItem data='Hello new user' msg='click here'/> -->
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
.center {
  position: absolute;
  top:  50%;
  left: 50%;
  transform: translate(-50%,-50%);
}

.testitem{
  position: relative;
  top:  505px;
  left: 50%;
  transform: translate(-50%,-50%);
}
</style>
