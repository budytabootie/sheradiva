<template>
	<main :class="`${link}-page`">
		<h1 :id="link">{{ head }}</h1>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Laboriosam alias, dignissimos veritatis molestias doloremque recusandae perspiciatis nulla exercitationem ratione consequatur aliquid maiores nostrum mollitia sapiente voluptates hic nobis ipsa commodi.</p>
<p>Doloribus exercitationem cupiditate nostrum repellendus error? Recusandae enim dolore temporibus dolor, est voluptatibus, non possimus voluptates quas consectetur excepturi ad eligendi iure ipsa nihil, rem unde reprehenderit officiis? Sed, rerum.</p>
<p>Ipsam dolores veniam illo eius. Reprehenderit dolore quasi, tempora quae nisi rem quos accusamus aperiam possimus eligendi magni magnam facere sunt excepturi corporis necessitatibus amet eius quaerat illo rerum corrupti?</p>
<p>Qui minus unde repellendus corporis excepturi exercitationem nostrum facere perferendis recusandae aperiam placeat aut tempora voluptas architecto, quaerat quae, odio error aliquid quos quod. Cum similique ad explicabo quidem sunt.</p>
<p>Error veniam nemo reiciendis illo fuga doloremque eligendi molestias minus. Quod obcaecati possimus impedit ab, eligendi neque pariatur alias quos ipsum sequi perspiciatis quasi nam. Animi aliquid dolor neque sequi?</p>
<p>Laboriosam mollitia, recusandae dolore dicta voluptas in! Omnis eius neque repellat adipisci nobis obcaecati et sint recusandae, nisi maxime sit quidem deserunt eaque natus repudiandae, alias perferendis at consequuntur. Incidunt.</p>
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
	color: purple;
}
</style>