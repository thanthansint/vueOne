<template>
    <div id="body2" v-on:click="display"><h1 id="text">Click Here!</h1>
    <div id="dis" ></div>
    
    </div> 
        
</template>

<script>
export default {
  name: 'Body2',  
  methods: {
      display: function () {
          document.getElementById('dis').style.position ="relative";
          document.getElementById('dis').style.top = "1vh";
          document.getElementById('dis').style.left = "1vw";
          document.getElementById('dis').style.width ="58vw";
          document.getElementById('dis').style.height = "13vh";
          document.getElementById('dis').style.background = "purple";
      }
}
}
</script>

<style scoped>
    #body2 {
        position: relative;
        top: 10vh;
        left: 20vw;
        width : 60vw;
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