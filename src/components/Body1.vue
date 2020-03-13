<template>
    <div id="mysubbody1">
    <p id="display"></p>
    <button id="click1" v-on:click="click1">Insert Text</button>
    <button id="tab" v-on:click="tabbing">Tab</button>
    </div>    
</template>

<script>
export default {
  name: 'Body1',
  data: function () {
    var tableft=1;     
    return (tableft);
  },
  methods: {
      click1: function Insert() {
        document.getElementById('click1').hidden ="true";
        document.getElementById('display').innerText = "This is a sub body 1";
        document.getElementById('display').style.fontSize = "30px";
        document.getElementById('display').style.color = "blue";
      },
      tabbing: function () {
          if (this.tableft) {
              document.getElementById('display').style.textAlign = "right";
              this.tableft = 0;
          } else {
              document.getElementById('display').style.textAlign = "left";
              this.tableft = 1;
          }          
      }
  }
}

</script>

<style scoped>
    #mysubbody1 {
        position: relative;
        top: 5vh;
        left: 10vw;
        width : 80vw;
        height : 15vh;
        border : 1px solid black; 
        background-color: yellow;    
    }  
    #click1, #tab {
        font-size: 20px;        
        position: relative;
        top: 25%;
        margin-right: 30px;
        padding: 10px 25px;
        background: blue;
        color: white;
    }
    
</style>