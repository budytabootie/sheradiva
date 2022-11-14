<template>
	<main>
		<article>
			<h1>This is an articles</h1>
			<section v-for="(header, index) in headers" :key="index" id="theSection">
				<h2 :id="header.link">{{ header.head }}</h2>
				<p>
					bangsat enim incididunt ea velit aliqua occaecat pariatur eu minim veniam. Duis fugiat ullamco amet
					cupidatat deserunt veniam incididunt. Ea eu in incididunt aute. Aliquip esse officia et magna sint
					ad incididunt id. Deserunt id enim dolor fugiat cillum mollit consequat eiusmod aliqua amet tempor
					sunt sint.

					Commodo officia ad labore exercitation dolor do ullamco. Esse do id aliqua tempor tempor ullamco
					consectetur ullamco qui. Eiusmod non in pariatur ipsum laboris laboris. Sunt pariatur veniam veniam
					occaecat non enim commodo elit consectetur commodo ipsum minim. Do pariatur ullamco deserunt ad do
					duis. Proident enim tempor est nostrud irure.

					Do ullamco exercitation proident irure ad reprehenderit consectetur adipisicing. Commodo culpa minim
					ut est. Ex minim veniam culpa deserunt officia ipsum adipisicing adipisicing. Sit commodo veniam
					exercitation exercitation consectetur cillum deserunt occaecat. Labore tempor duis consequat aliquip
					sunt reprehenderit elit non Lorem proident velit adipisicing consequat. Sunt nostrud exercitation
					ullamco ex irure aute. Adipisicing elit do aliquip ipsum id deserunt excepteur proident quis qui.

					Veniam exercitation duis aliqua dolore proident Lorem aute minim nostrud nostrud sit. Nostrud elit
					ex id in aliquip cillum cillum dolore deserunt et. Consequat magna minim minim occaecat Lorem enim
					labore ut aliqua eiusmod. Aliquip irure pariatur qui mollit officia culpa adipisicing elit sit
					nostrud aliquip.

					Ut ullamco sint tempor voluptate commodo minim adipisicing laboris. Pariatur ipsum consequat culpa
					reprehenderit. Dolore voluptate deserunt do ex do eiusmod irure Lorem pariatur enim excepteur dolore
					mollit aute.

					Laboris consectetur minim proident exercitation et in excepteur eu quis officia nostrud eu. Minim
					est ullamco adipisicing velit esse quis exercitation proident tempor commodo qui adipisicing.
					Laboris consequat proident id proident sunt ullamco eu.

					Consequat qui magna duis mollit labore do est laboris occaecat. Culpa eiusmod ipsum esse dolore ex
					et exercitation consectetur qui in veniam adipisicing enim. Sint occaecat Lorem qui excepteur eu.
					Sit ex veniam id proident. Eu non cillum consectetur do cillum officia duis non. Magna minim aliquip
					est voluptate deserunt duis anim Lorem Lorem irure.

					Duis commodo anim ea dolor deserunt et sit exercitation excepteur cillum eiusmod sunt. Aliquip
					mollit elit magna proident velit ex culpa ullamco labore commodo Lorem id esse. Excepteur irure
					labore eu cillum consequat et minim nisi non.

					Eu quis deserunt exercitation incididunt mollit. Pariatur cupidatat do reprehenderit ut consectetur
					pariatur laborum reprehenderit consectetur eiusmod sunt quis nisi laboris. Minim id qui velit
					nostrud occaecat fugiat occaecat sunt deserunt proident Lorem do. Do consectetur et deserunt aute
					fugiat aute reprehenderit.

					Nostrud reprehenderit id magna excepteur magna proident ullamco velit cillum excepteur magna.
					Proident nulla eu cupidatat consectetur reprehenderit enim labore. Elit culpa proident ipsum aliquip
					anim irure cupidatat ut incididunt nisi sint aute. Irure aliqua laboris in veniam exercitation
					consectetur proident. Aliqua esse duis nostrud sint est. Nostrud irure velit ex duis dolore anim.
				</p>
			</section>
		</article>
	</main>
</template>

<script setup>
import { ref, onMounted } from 'vue'

const headers = [
	{ "head" : "About", "link" : "About"},
	{ "head" : "Product", "link" : "Product"},
	{ "head" : "Web Development", "link" : "Web-Development"},
	{ "head" : "Web Applications", "link" : "Web-Applications"},
	{ "head" : "Web Portals", "link" : "Web-Portals"},
	{ "head" : "Mobile Applications", "link" : "Mobile-Applications"},
	{ "head" : "Telegram Bot", "link" : "Telegram-Bot"},
	{ "head" : "Maintenance Support", "link" : "Maintenance-Support"}
]

const currentSection = ref('')


onMounted(() => {
	const observer = new IntersectionObserver((entries) => {
		entries.forEach((entry) => {
			if (entry.intersectionRatio > 0) {
				currentSection.value = entry.target.getAttribute('id')
			}
		})
	},
		{
			rootMargin: '0px 0px -90% 0px',
		})
	document.querySelectorAll('article h2').forEach((section) => {
		observer.observe(section)
	})

})

</script>

<style lang="scss" scoped>
html {
  scroll-behavior: smooth;
}

main {
	display: flex;
}

article {
	width: 75%;
	margin-bottom: 500px;

	section {
		padding: 50px 0 50px 0px;
	}
}

aside {
	width: 25%;

	a {
		display: block;
		color: #2c3e50;
		text-decoration: none;
		border-left: 1px solid #ccc;
		padding-left: 2em;

		&.active {
			font-weight: bold;
			border-color: black;
		}
	}

	div {
		position: sticky;
		top: 20px;
		padding-left: 2em;
	}
}
</style>