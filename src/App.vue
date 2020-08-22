<template>
  <span >
    <header>
      <nav-bar logo="Social" url="#" cor="blue" />
    </header>

    <main>
      <div class="container">
        <div class="row">

          <grid-vue tamanho="4">
            <div class="card-panel grey lighten-5 z-depth-1">
              <div class="row valign-wrapper">
                <div class="col s4">
                  <img src="https://materializecss.com/images/yuna.jpg" alt="" class="circle responsive-img"> <!-- notice the "circle" class -->
                </div>
                <div class="col s8">
                  <span class="black-text">
                    <h5>Maria Silva</h5>
                    Add the "circle" class to it to make it appear circular.
                  </span>
                </div>
              </div>
            </div>
          </grid-vue>

          <grid-vue tamanho="8">
            <router-view/>
          </grid-vue>

        </div>
      </div>
    </main>

<div class="footer">
      <footer-vue cor="blue" logo="Social" descricao="Teste de descrição" ano="2018">

      <li><a class="grey-text text-lighten-3" href="#!">Home</a></li>
      <li><a class="grey-text text-lighten-3" href="#!">Link 2</a></li>
      <li><a class="grey-text text-lighten-3" href="#!">Link 3</a></li>
      <li><a class="grey-text text-lighten-3" href="#!">Link 4</a></li>

    </footer-vue>

</div>



  </span>
</template>

<script>
import NavBar from '@/components/layouts/NavBarVue'
import FooterVue from '@/components/layouts/FooterVue'
import GridVue from '@/components/layouts/GridVue'

export default {
  name: 'app',
  components:{
    NavBar,
    FooterVue,
    GridVue
  }
}
</script>

<style>
.footer {
  position: fixed;
  left: 0;
  bottom: 0;
  width: 100%;
}


</style>
