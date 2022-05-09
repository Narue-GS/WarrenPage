<template>
  <div class="box" v-if="fase==1">
  <Fase1 />
  </div>
  <div class="box" v-if="fase==2">
  <h1>AAAaaa</h1>
  </div>
  <BotaoM msg="Proximo" id="proximo" v-on:click='next' />
</template>

<script>
  import BotaoM from "./B/BotaoM.vue"
  import Fase1 from "./fases/fase1.vue"
    export default {
        components:{
            BotaoM,
            Fase1,
        },
        data() {
          return {
            fase:1
          }
        },
        methods: {
        next: function(){
          if(this.fase >= 3){
            this.fase = 3
          }
          else{
              this.fase += 1
              
            } 
          }
        },
      }

    
    
</script>


<style scoped>

    div{
      position: absolute;
    }

  .box{
    box-sizing: border-box;
    width: 35%;
    height: 100%;
    margin:4% 15%;
    text-align: left;
    padding: 1%;
    
  }

  #proximo{
    margin-top: 63%;
    font-size: 150%;
    margin-left:15%;
    width:10%;
    height: 100%;
    padding: 1%;

  }

  
</style>