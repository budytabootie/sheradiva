<template>
	<main>
		<article>
			<section v-for="(header, index) in headers" :key="index" id="theSection">
				<component :is="header.component" :head="header.head" :link="header.link" :data="headers"></component>
			</section>
		</article>
	</main>
</template>

<script setup>
import { ref, onMounted } from 'vue'
import About from './pages/About.vue'
import Product from './pages/Product.vue'
import Web_Development from './pages/Web_Development.vue'
import Web_Applications from './pages/Web_Applications.vue'
import Web_Portals from './pages/Web_Portals.vue'
import Mobile_Applications from './pages/Mobile_Applications.vue'
import Telegram_Bot from './pages/Telegram_Bot.vue'
import Maintenance_Support from './pages/Maintenance_Support.vue'

const headers = [
	// { "head" : "Web Portals", "link" : "Web-Portals", "component" : Web_Portals},
	// { "head" : "Mobile Applications", "link" : "Mobile-Applications", "component" : Mobile_Applications},
	{ "head" : "About", "link" : "About", "component" : About},
	{ "head" : "Product", "link" : "Product", "component" : Product},
	// { "head" : "Web Development", "link" : "Web-Development", "component" : Web_Development},
	// { "head" : "Web Applications", "link" : "Web-Applications", "component" : Web_Applications},
	// { "head" : "Web Portals", "link" : "Web-Portals", "component" : Web_Portals},
	// { "head" : "Mobile Applications", "link" : "Mobile-Applications", "component" : Mobile_Applications},
	// { "head" : "Telegram Bot", "link" : "Telegram-Bot", "component" : Telegram_Bot},
	// { "head" : "Maintenance Support", "link" : "Maintenance-Support", "component" : Maintenance_Support}
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