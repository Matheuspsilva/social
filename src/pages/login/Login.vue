<template>
  <template-login>

    <span slot="menuesquerdo">
      <img src="https://image.freepik.com/free-vector/mobile-login-concept-illustration_114360-83.jpg" alt="" class="responsive-img" id="login-img">
    </span>

      <span slot="principal">
        <span v-if="!cadastro">
          <h2>Login</h2>

          <input type="text" placeholder="Email">
          <input type="password" placeholder="Password">
          <button  class="btn blue waves-effect waves-light">Entrar</button>
          <button  class="btn light-blue lighten-2 waves-effect waves-light" v-on:click="cadastro = !cadastro">Cadastre-se</button>

        </span>

        <span v-if="cadastro">
          <h2>Cadastro</h2>

          <input type="text" placeholder="Nome">
          <input type="text" placeholder="Email">
          <input type="password" placeholder="Senha">
          <input type="password" placeholder="Confirme sua Senha">

          <button  class="btn blue waves-effect waves-light">Cadastrar</button>
          <button  class="btn light-blue lighten-2 waves-effect waves-light" v-on:click="cadastro = !cadastro">Já possuo conta</button>

        </span>
      </span>


  </template-login>

</template>

<script>

import TemplateLogin from '@/templates/TemplateLogin'



export default {
  name: 'Login',
  data () {
    return {
      cadastro:false
    }
  },
    components:{
      TemplateLogin

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#login-img{
  margin-top: 5px;
}

</style>
