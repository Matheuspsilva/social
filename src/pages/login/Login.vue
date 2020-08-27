<template>
  <template-login>

      <h2>Login</h2>

      <input type="text" placeholder="email">
      <input type="password" placeholder="password">
      <button class="btn">Entrar</button>

  </template-login>

</template>

<script>
import CardConteudoVue from '@/components/social/CardConteudoVue'
import CardDetalheVue from '@/components/social/CardDetalheVue'
import PublicarConteudoVue from '@/components/social/PublicarConteudoVue'
import TemplateLogin from '@/templates/TemplateLogin'



export default {
  name: 'Login',
  data () {
    return {

    }
  },
    components:{
      CardConteudoVue,
      CardDetalheVue,
      PublicarConteudoVue,
      TemplateLogin

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
