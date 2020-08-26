<template>

<div class="row">
      <grid-vue class="input-field col s12" tamanho="12">
        <textarea v-model="conteudo" class="materialize-textarea"></textarea>
        <label >O que está acontecendo?</label>
      </grid-vue>
      <div>
        <grid-vue v-if="conteudo" class="btn blue waves-effect waves-light" tamanho="2 offset-s10">Publicar</grid-vue>
      </div>
    </div>


</template>

<script>
import GridVue from '@/components/layouts/GridVue'

export default {
  name: 'PublicarConteudoVue',
  props:[],
  data () {
    return {
      conteudo:''

    }
  },
    components:{
      GridVue
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
