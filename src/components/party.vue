<template>
    <div id="party-container" v-on:click="party">
    <h1 >Party</h1>
  </div>
</template>

<script>
export default {
  name: 'party',
  methods: {
    party: function () {
        function getRandomColor(){
          let index=Math.floor(Math.random()*3);
          let colors=["red", "blue", "orange"];
          return colors[index];
        }
        
        setInterval(function(){
            document.getElementById('party-container').style.background = getRandomColor();
        }, 100);
   
    }
  }
}

</script>

<style scoped>
    #party-container {        
        width : 10vw;
        height : 15vh;        
        border : 1px solid black; 
        text-align: center;
    }  
</style>