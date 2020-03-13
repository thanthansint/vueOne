<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Tweet author="Than" content="This is a tweet" date="2020-03-12"/> -->
    <myheader/>
    <myfooter/>
    <mybody/>
  </div>
</template>

<script>

import myheader from './components/Header.vue'
import myfooter from './components/Footer.vue'
import mybody from './components/Body.vue'

export default {
  name: 'App',
  components: {
    myfooter,
    myheader,
    mybody    
  }
}
</script>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

#app {
  
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;  
  color: #2c3e50;
  margin-top: 0px;
  
}
</style>
