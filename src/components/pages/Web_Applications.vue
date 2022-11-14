<template>
	<main :class="`${link}-page`">
		<h1 :id="link">{{ head }}</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea molestias quod praesentium cum corporis dolorum. Odio voluptatibus dicta recusandae animi deleniti quaerat ex delectus? Explicabo error harum nam natus debitis!</p>
<p>Nisi facere nemo similique vero natus iste alias dicta, rem tempora, itaque harum qui exercitationem ratione atque ullam expedita? Necessitatibus labore atque commodi architecto excepturi fugiat fuga illum beatae voluptatum.</p>
<p>Veritatis corporis doloribus vitae error distinctio voluptatum, possimus, libero pariatur vero aliquam voluptatem sit qui, id sunt repudiandae? Aliquid in incidunt qui maxime, temporibus minima quas nesciunt at expedita doloremque!</p>
<p>Porro amet vero sint repudiandae suscipit voluptas numquam consequatur debitis itaque illo, rem quisquam, deserunt et! Quos assumenda beatae, totam odit ducimus iste voluptatum voluptas quas deleniti quo reprehenderit a.</p>
<p>Officia dolorum est cum nihil, deleniti saepe animi quis quos veritatis assumenda atque esse quidem eaque accusantium culpa minus deserunt, fugiat porro facere autem dolor eum error sequi. Odit, fugit?</p>
<p>Aut, corrupti quibusdam! Est ab quos, itaque ad voluptatum quisquam magni ratione praesentium iusto, dolore fugiat rem deserunt voluptatibus quas sapiente, reiciendis unde facilis porro? Illum consequuntur natus voluptatem maxime.</p>
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
	color: black;
}
</style>