<template>
    <div>
        <img alt="progresso" src="@/assets/linha.png" width="580" height="25">
        <h1 id="a" v-on:click="next">Seja bem-vindo</h1><br>
        <span>Quetal começar a investir do melhor jeito? Primeiro nos conte sobre você para
       depois contarmos sobre o jeito Warren de investir!</span>
      <form>
            <label for="nome" class='especialLabel'>NOME COMPLETO</label><br>
            <input type="text-box" id="nome" name="nome"><br>
        
            <div class="subBox1">
            
            <EmailIcon id="con"/>
            <label for="email" class='normalLabel'>EMAIL</label><br><br><br>
            <input type="email" class="inBox" id="emailBox1" name="email"><br>
            
            
            <label for="cpf" class='normalLabel'>CPF</label><br><br><br>
            <input type="text" class="inBox" id="cpf" name="cpf" autocomplete="off" maxlength="14"><br>
            
           
            <label for="date" class='normalLabel'>DATA DE NASCIMENTO</label><br><br><br>
            <input type="text" name="date" class="inBox" id="date">

            <strong>
            <p>Quer receber aszz melhores dicas e ficar por dentro do universo Warren?</p>
            <p>Então selecione por onde deseja recerber tudo e mais um pouco:</p><br><br><br>
            </strong>
            <input type="checkbox" id="checkin" name="msg">
            <label for="msg" id="check">Email e SMS</label><br><br><br>
            <label for="whats" id="check">Whatsapp</label>
            <input type="checkbox" id="checkin" name="whats"><br><br><br>

            <p>Quer receber as melhores dicas e ficar por dentro do universo Warren?</p>
            <p>Então selecione por onde deseja recerber tudo e mais um pouco:</p>

        
        </div>
        <div class="subBox2">
            
            <label for="email" class='normalLabel'>CONFIRMAR EMAIL</label><br><br><br>
            <input type="text-box" class="inBox" id="emailBox2" name="email"><br>
           
            
            <label for="email" class='normalLabel'>TELEFONE</label><br><br><br>
            <input type="text-box" class="inBox" id="" name="email"><br>
            
        </div>
      </form>

    </div>
</template>

<script>
import EmailIcon from "/src/components/icons/emailIcon.vue"
import DataIcon from "/src/components/icons/dataIcon.vue"
export default {
    components:{
        EmailIcon,
        DataIcon
    },
    
}
</script>

<style>
    #con{
    position:absolute;
    margin-top: 12.5%;
    margin-left: 2%;
  }

  #nome{
    
    width: 95%;
    height: 6em;
    padding: 12px 20px;
    display: inline-block;
    border-radius: 4%;
    box-sizing: border-box;
  }

  #check{
    position: absolute;
    margin-left: 10%;
    margin-top:0%;
  }

  #checkin{
    position: absolute;
    
    
  }

  .dateBox{
    border: solid 1px;
    width: 45%;
    margin-top: 7.5%;
    height: 5em;
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
  .inBox{
    border-color: none;
    border: solid 1px;
    z-index: -1;
    width: 45%;
    height: 6em;
    padding: 3px;
    
    border-radius: 4%;
    box-sizing: border-box;
  }

  #a{
    font-size: 350%;
    margin-bottom: 1%;
  }

  .normalLabel{
    z-index: 1;
    margin-left: 1%;
    position: absolute;
    background: white;
    position: absolute;
    margin-top: 7.5%;
    float: left;
    font-size: 70%;
    font-weight: 700;
  }

  .especialLabel{
    z-index: 1;
    margin-left: 1%;
    position: absolute;
    background: white;
    position: absolute;
    margin-top: 2%;
    float: left;
    font-size: 70%;
    font-weight: 700;
  }
</style>