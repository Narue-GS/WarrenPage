<template>
  <div class="corpo">
    <NavCadastro />
    <FormCadastro />
    
    <img  id="moça" alt="moça grande" src="@/assets/moçaGrande.png" width="621" height="1287" >
    
  </div>
</template>

<script setup>
import NavCadastro from '../components/NavCadastro.vue'
import FormCadastro from '../components/FormCadastro.vue'
</script>

<style>
  body{
    background-color: rgb(246, 253, 254);
    margin: 0%;
  }

  #moça{
    float: right;
  }
</style>
