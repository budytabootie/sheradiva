<template>
	<main :class="`${link}-page`">
		<h1 :id="link">{{ head }}</h1>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Cumque impedit dolore incidunt quod, dolor nemo consequuntur mollitia ad illum aliquam dolorem unde ipsam vel animi voluptatibus ratione inventore ut nostrum.</p>
<p>Corrupti, quibusdam et illo labore quos modi? Enim consequuntur ad quisquam nisi sit iusto mollitia suscipit tempora sunt nesciunt. Magnam quibusdam dolorem tempora sapiente corporis doloremque, aliquam consequatur architecto reiciendis!</p>
<p>Nisi maxime voluptatum tempora sint. Distinctio iusto reiciendis sequi sunt sapiente! Dolores dolor qui voluptates blanditiis nobis velit asperiores maxime hic. Est, in. Maiores totam est impedit rem ipsam dolorem!</p>
<p>Fugit debitis temporibus suscipit nemo nulla vero nisi eaque aut ullam rem ea cumque eligendi, in commodi laborum cum illum voluptatum, repellendus eveniet! Magni ex sequi suscipit obcaecati ea voluptate.</p>
<p>Quisquam accusamus eveniet nam necessitatibus officia eos ex cumque adipisci molestias ab. Eveniet quis vitae mollitia voluptates non reiciendis! Perspiciatis ipsum culpa sunt sint sapiente! Inventore sequi maiores neque vero?</p>
<p>Quo suscipit dolor praesentium mollitia, quae eligendi optio similique voluptas, ex velit tempora voluptatem inventore distinctio quia pariatur dicta. Ab sequi, corrupti quaerat excepturi veritatis qui ea unde nemo autem.</p>
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
	color: orange;
}
</style>