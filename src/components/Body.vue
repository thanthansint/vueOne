<template>
    <div id="body-container">
      <button id="click" v-on:click="clickhere">Change Body Color Here!!</button>      
        <subbody1/>
        <subbody2/>
        <subbody3/>
    </div>
     
</template>

<script>
import subbody1 from './Body1.vue'
import subbody2 from './Body2.vue'
import subbody3 from './Body3.vue'


export default {
  name: 'Body',
  data: function () {
    var count=0; 
    return count;
  },
  components: {
    subbody1,
    subbody2,
    subbody3
  },
  methods: {
    clickhere: function () {
      if (this.count==0) {
        document.getElementById('body-container').style.background="green"; 
      }else if (this.count == 1) {
              document.getElementById('body-container').style.background="orange"; 
            } else {
              document.getElementById('body-container').style.background="white"; 
              this.count =0;
              return;
            }
            this.count++;
  }  
  }
}

</script>

<style scoped>
    #body-container {
        position: absolute;
        top: 15vh;
        width : 100vw;
        height : 75vh;
        border : 1px solid black; 
        background-color: pink;    
    }  
    #click {
      width: 30vw;
      height: 10vh;
      font-size: 20px;
      color: white;
      background: black;
    }
</style>