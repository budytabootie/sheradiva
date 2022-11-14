<template>
	<main :class="`${link}-page`">
		<h1 :id="link">{{ head }}</h1>
		<p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Fugiat id vel laboriosam itaque quisquam impedit quos accusantium quae! Magni id laborum accusamus qui ipsa vitae dolores excepturi beatae ad explicabo.</p>
<p>Exercitationem quos dolorum quis laborum. Quasi inventore beatae cumque ducimus quod repellat! Totam harum delectus dolore, saepe rem maiores eaque culpa minus voluptatibus, laudantium quo necessitatibus sapiente vel esse hic.</p>
<p>Explicabo quod minima vel, iure tempore aperiam at deleniti dolores dolorem dicta cumque consequuntur eos molestias saepe, blanditiis natus. Mollitia vel cum ipsum sit explicabo ab adipisci, ducimus voluptatem distinctio!</p>
<p>Adipisci, sequi? Eos hic eveniet doloremque quis animi. Earum, similique accusantium sapiente suscipit vel in. Aut rem fuga voluptas quasi blanditiis eligendi, ullam quaerat quo officia dolore nobis velit minus.</p>
<p>Odit ut deserunt, ducimus sit debitis error molestiae aspernatur animi facilis. Perspiciatis libero voluptate, reiciendis, ipsa accusantium distinctio tenetur error similique debitis assumenda ex ipsam aliquid. Nostrum nisi deleniti rem!</p>
<p>Veritatis nobis quae sit ipsam! Eum veniam accusamus velit nemo, culpa ipsum, at voluptates sapiente omnis temporibus, quisquam adipisci nihil reiciendis tempore quo vel quod cum molestias optio quibusdam quas.</p>
	</main>
</template>

<script setup>
// import { props } from 'vue'

const props = defineProps({
	data: {
		type: Array
	},
	head: {
		type: String
	},
	link: {
		type: String
	}
})
</script>

<style lang="scss" scoped>
h1 {
	color: green;
}
</style>