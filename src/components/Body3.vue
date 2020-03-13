<template>
    <div id="body3" v-on:click="sub3"><h1 id="text">SubBody3</h1></div>     
</template>

<script>
export default {
  name: 'body3',
  methods: function () {
      document.getElementById('text').style.color = 'red';
      
  }
}
</script>

<style scoped>
    #body3 {
        position: relative;
        top: 15vh;
        left: 30vw;
        width : 40vw;
        height : 15vh;
        border : 1px solid black; 
        background-color: yellow;    
    }  
    #text {
        position: absolute;
        top: 25%;
        left: 40%;
    }  
</style>