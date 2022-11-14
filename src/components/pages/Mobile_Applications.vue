<template>
	<main :class="`${link}-page`">
		<h1 :id="link">{{ head }}</h1>
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quidem at minus reiciendis debitis recusandae. Numquam quae voluptate aut quisquam earum dolore adipisci vero nostrum in, repudiandae unde quibusdam perferendis suscipit!</p>
<p>Quo non et alias blanditiis impedit dolorum est magni amet quis. Laboriosam beatae perferendis quos quae quam nihil molestias illo est maiores sit incidunt minima unde, voluptatibus voluptatem quia inventore!</p>
<p>Molestias sed aspernatur eligendi, perferendis nobis necessitatibus veniam vel a eveniet ab. Reprehenderit at, sunt ex natus et molestias veniam aspernatur excepturi iusto. Quam nemo tempora veniam ipsum dolor voluptatem.</p>
<p>Quod dolorum, animi laborum fugiat, officia inventore a magni minus vero ut eveniet sunt magnam voluptatum deleniti porro temporibus, eum odit. Sequi est unde, praesentium impedit rem amet illo distinctio.</p>
<p>Ad deserunt possimus dolore, eaque eum officiis laudantium amet voluptate. Corrupti optio quisquam sequi nam, voluptate pariatur iste iusto at id voluptatibus ratione, eaque culpa enim dolore unde ducimus quod.</p>
<p>Voluptates vel vitae quae hic quis minima tempora. Vero, quod itaque ipsum optio nemo provident harum fuga nisi natus deserunt labore obcaecati accusantium soluta expedita incidunt nobis, nulla commodi quibusdam?</p>
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
	color: blue;
}
</style>