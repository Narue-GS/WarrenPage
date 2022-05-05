<template>
  <div class="navbar">
    <p id="title">FORMULÁRIO</p>
    
  </div>
   
    
</template>

<script>
export default {
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .navbar {
    background-color: rgb(255, 26, 95);
    display: flex;
    justify-content: space-evenly;
    padding-bottom: 0px;
    height:1.5em;
    font-size: 30px;
    margin-bottom: 0%; 
    text-align: center;  color: azure; 
    }

    p{
      margin-top: 0.8%;
      font-size: 45%;
      font-weight: 700;

    }
</style>
