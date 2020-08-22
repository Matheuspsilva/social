<template>
  <span >
    <header>
      <nav-bar logo="Social" url="#" cor="blue" />
    </header>

    <main>
      <div class="container">
        <div class="row">

          <grid-vue tamanho="4">

            <card-menu-vue>
              <div class="row valign-wrapper">
                <grid-vue tamanho="4">
                  <img src="https://materializecss.com/images/yuna.jpg" alt="" class="circle responsive-img"> <!-- notice the "circle" class -->
                </grid-vue>
                 <grid-vue tamanho="8">
                  <span class="black-text">
                    <h5>Maria Silva</h5>
                    Add the "circle" class to it to make it appear circular.
                  </span>
                </grid-vue>
              </div>
            </card-menu-vue>

            <card-menu-vue>
              <h3>Teste</h3>
            </card-menu-vue>

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
import CardMenuVue from '@/components/layouts/CardMenuVue'


export default {
  name: 'app',
  components:{
    NavBar,
    FooterVue,
    GridVue,
    CardMenuVue
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
