<template>
	<main :class="`${link}-page`">
		<h1 :id="link">{{ head }}</h1>
		<p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Magni voluptate praesentium enim earum, reprehenderit placeat maiores, incidunt dignissimos temporibus ipsum ea, suscipit cupiditate possimus iusto error voluptatum explicabo beatae necessitatibus.</p>
<p>Ratione eaque, accusantium inventore rem vel necessitatibus temporibus aliquam ipsa, sapiente cum tempore officia dolorem tempora ex ullam odit ad recusandae distinctio eum vero consequatur, possimus dicta magnam molestias! Iure.</p>
<p>Tenetur molestias illum porro, ipsam ad totam numquam quidem adipisci unde nesciunt voluptas? Animi, voluptas deserunt exercitationem blanditiis ex dolores natus. Esse ex natus maxime dolorem et, eius odio molestiae.</p>
<p>Perspiciatis voluptates obcaecati ab? Expedita saepe dolores repudiandae quas doloremque dolor eius adipisci accusantium vero minima modi ratione voluptate voluptatum laboriosam ipsam ipsum, aliquam autem harum quod dignissimos quisquam ab!</p>
<p>Esse nobis impedit corporis provident quod molestiae dolores, quae officiis asperiores sint culpa tempore voluptas, voluptatum eum recusandae, quia eveniet saepe consequatur autem magnam laboriosam beatae reprehenderit fuga? Quis, consequatur!</p>
<p>Quam consequuntur fuga perferendis possimus repellat vel unde enim modi architecto? Cum recusandae ipsa, deserunt repudiandae voluptatem sint nisi, maxime fuga in et accusantium eius placeat deleniti aut necessitatibus? Recusandae!</p>
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
	color: yellow;
}
</style>