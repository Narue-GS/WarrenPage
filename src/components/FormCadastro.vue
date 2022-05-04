<template>
  <div class="box">
    <img alt="progresso" src="@/assets/linha.png" width="580" height="25">
    <h1 id="a" v-on:click=test>Seja bem-vindo</h1><br>
    <span>Quetal começar a investir do melhor jeito? Primeiro nos conte sobre você para
       depois contarmos sobre o jeito Warren de investir!</span>
      <form action="/">
        <label for="nome" class='especialLabel'>NOME COMPLETO</label><br>
        <input type="text-box" id="nome" name="nome"><br>
      </form>
      <div class="subBox1">
        <form action="/">
          <label for="email" class='normalLabel'>EMAIL</label><br><br><br>
          <input type="email" class="inBox" id="emailBox1" name="email"><br>
        </form>
        <form>
          <label for="cpf" class='normalLabel'>CPF</label><br><br><br>
          <input type="text" class="inBox" id="cpf" name="cpf" autocomplete="off" maxlength="14"><br>
        </form>
        <label for="date" class='normalLabel'>DATA DE NASCIMENTO</label><br><br><br><br>
        <input type="text" name="date" class="inBox" id="date"><br><br><br>
        <strong>
          <p>Quer receber as melhores dicas e ficar por dentro do universo Warren?</p>
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
        <form action="/">
          <label for="email" class='normalLabel'>CONFIRMAR EMAIL</label><br><br><br>
          <input type="text-box" class="inBox" id="emailBox2" name="email"><br>
        </form>
        <form action="/">
          <label for="email" class='normalLabel'>TELEFONE</label><br><br><br>
          <input type="text-box" class="inBox" id="" name="email"><br>
        </form>
      </div>
        <RouterLink to="/"><BotaoM msg="Proximo" id="proximo"/></RouterLink>
        
  </div>
</template>

<script>
  import BotaoM from "./B/BotaoM.vue"
    export default {
        components:{
            BotaoM
        },
        // verifica(){
        //   const input = document.querySelector('#cpf')

        //   input.addEventListener('keypress', () => {
        //     let inputlength = input.value.length

        //     if(inputlength === 3) {
        //       input
        //     }
        //   })
        // }
        
    }
  
//   input.addEventListener('keypress', () =>{
//     let inputlength = input.value.length

//     if(inputlength = 0){
//         alert(aaa)
//     }
// })

    
    
</script>


<style scoped>

  #proximo{
    margin-top: 128%;
    font-size: 150%;
    width:25%;
    height: 10%;
    padding: 1%;

  }

  #nome{
    
    width: 100%;
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
.lNome{
  
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
    z-index: -1;
    width: 45%;
    height: 6em;
    padding: 0px;
    display: inline-block;
    border-radius: 4%;
    box-sizing: border-box;
  }

  .box{
    position: absolute;
    box-sizing: border-box;
    width: 35%;
    margin:4% 15%;
    text-align: left;
    padding: 1%;
    
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
  
  margin-top: 5%;
  float: left;
  font-size: 70%;
  font-weight: 700;
}


  
</style>