<template>
  <div class="box">
    <img alt="progresso" src="@/assets/linha.png" width="580" height="25">
    <h1 id="a">Seja bem-vindo</h1><br>
    <span>Quetal começar a investir do melhor jeito? Primeiro nos conte sobre você para
       depois contarmos sobre o jeito Warren de investir!</span>
      <form action="/">
        <label for="nome">NOME COMPLETO</label><br>
        <input type="text-box" id="nome" name="nome"><br>
      </form>
      <div class="subBox1">
        <form action="/">
          <label for="email">EMAIL</label><br><br><br>
          <input type="email" id="inBox" name="email"><br>
        </form>
        <form action="/">
          <label for="email">CPF</label><br><br><br>
          <input type="text-box" id="inBox" name="email"><br>
        </form>
        <label for="date">DATA DE NASCIMENTO</label><br><br><br><br>
        <input type="date" name="date" id="date">
        <p>Quer receber as melhores dicas e ficar por dentro do universo Warren?</p>
        <p>Então selecione por onde deseja recerber tudo e mais um pouco:</p>
        <input type="checkbox" name="msg">
        <label for="msg">Email e SMS</label><br><br><br>
        
         
        <input type="checkbox" name="whats">
       
      </div>
      <div class="subBox2">
        <form action="/">
          <label for="email">CONFIRMAR EMAIL</label><br><br><br>
          <input type="text-box" id="inBox" name="email"><br>
        </form>
        <form action="/">
          <label for="email">TELEFONE</label><br><br><br>
          <input type="text-box" id="inBox" name="email"><br>
        </form>
      </div>
  </div>
</template>

<script>

</script>


<style scoped>

  #nome{
    width: 100%;
    height: 6em;
    padding: 12px 20px;
    margin-top:1%;
    display: inline-block;
    border-radius: 4%;
    box-sizing: border-box;
}

  .subBox1{
    display: flexbox;
    position: absolute;
    width: 98%;
    text-align: left;

  }

  .subBox2{
    display: flexbox;
    position: absolute;
    margin-left: 50%;
    width: 98%;
  }
  #inBox{
    width: 45%;
    height: 6em;
    padding: 12px 20px;
    display: inline-block;
    border-radius: 4%;
    box-sizing: border-box;
  }

  .box{
    position: absolute;
    width: 35%;
    margin:4% 15%;
    text-align: left;
    padding: 1%;
    
}

#a{
  font-size: 350%;
  margin-bottom: 1%;
}
.box label{
  margin-top: 5%;
  margin-bottom: 0%;
  float: left;
  font-size: 70%;
  font-weight: 700;
}


  
</style>