<template>
	<span>
		<header>
			<nav-bar logo="Fakebook" url="/" cor="blue" >
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/login">Login</router-link></li>
			</nav-bar>
		</header>

		<main>
			<div class="container">
				<div class="row">
					<grid-vue tamanho="6">
						  <slot name="menuesquerdo"/>
					</grid-vue>
					<grid-vue tamanho="6">
						<slot name="principal"/>
					</grid-vue>
				</div>
			</div>
		</main>

		<footer-vue cor="blue" logo="Social" descricao="Teste de descrição" ano="2018">

			<li><a class="grey-text text-lighten-3" href="#!">Home</a></li>
			<li><a class="grey-text text-lighten-3" href="#!">Link 2</a></li>
			<li><a class="grey-text text-lighten-3" href="#!">Link 3</a></li>
			<li><a class="grey-text text-lighten-3" href="#!">Link 4</a></li>

		</footer-vue>

	</span>
</template>

<script>
import NavBar from '@/components/layouts/NavBarVue'
import FooterVue from '@/components/layouts/FooterVue'
import GridVue from '@/components/layouts/GridVue'
import CardMenuVue from '@/components/layouts/CardMenuVue'




export default {
	name: 'TemplateLogin',
	components:{
		NavBar,
		FooterVue,
		GridVue,
		CardMenuVue
	}
}
</script>

<style>


</style>
