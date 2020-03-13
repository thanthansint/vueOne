<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Tweet author="Than" content="This is a tweet" date="2020-03-12"/> -->
    <header/>
  <div id="party">
    <button>Party</button>
  </div>
    
  </div>
</template>

<script>

import header from './components/header.vue'
import party from './components/party.vue'

export default {
  name: 'App',
  components: {
    header,
    party
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
