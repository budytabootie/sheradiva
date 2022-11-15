<template>
	<main :class="`${link}-page`">
		<h1 :id="link">{{ head }}</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus laboriosam sequi maiores quidem modi dolore cumque reiciendis laudantium nulla beatae ea, cupiditate eum veritatis dicta itaque eligendi aliquid. Sint, deserunt!</p>
<p>Excepturi dolores eius quas earum iusto autem optio et, molestiae laboriosam tenetur fuga numquam labore quae repellat praesentium, sequi quos, veritatis aliquid? Distinctio autem similique culpa, blanditiis ea praesentium sint!</p>
<p>Iure suscipit ipsum, neque soluta modi quisquam eveniet iste atque quidem enim delectus, numquam quas, dignissimos consequatur libero itaque totam esse expedita nulla. Quia perspiciatis id amet molestias blanditiis! Placeat?</p>
<p>Labore, dignissimos modi facere rerum voluptatibus illum magni ipsa doloremque vero aliquid dolor doloribus fuga provident, non vitae, numquam alias. Iure, iusto tempore culpa eius perspiciatis sint quidem saepe assumenda!</p>
<p>Culpa temporibus quaerat dolore velit assumenda perferendis cumque iure! Quos expedita nemo neque, dolorum iure voluptate quod repudiandae cupiditate. Maiores animi consectetur facere earum aperiam nobis adipisci expedita. Non, fuga.</p>
<p>Officiis quasi minima sequi! Impedit, praesentium quaerat voluptates amet ipsa quia saepe neque labore quo eligendi provident. Vel nihil molestiae, reiciendis tenetur mollitia consequuntur recusandae dolorem ullam et in. Veniam.</p>
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
	color: brown;
}
</style> 