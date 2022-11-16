<template>
	<!-- SIDEBAR -->
	<div class="app">
		<Sidebar />
		<main>
			<Content />
		</main>
		<!-- <router-view /> -->
	</div>
</template>
<script setup>
import Sidebar from './components/Sidebar.vue';
import Content from './components/Content.vue';
</script>
<style lang="scss">
:root {
	--primary: #4ade80;
	--grey: #64748b;
	--light-alt: #F3F5FA;
	--dark-alt: #334155;
	--light: #FFFFFF;
	--sidebar-width: 300px;
	--light-blue: #C2C1FB;
}

* {
	margin: 0;
	padding: 0;
	box-sizing: border-box;
	font-family: 'Fira sans', sans-serif;
}

body {
	background: var(--light);
}

body::-webkit-scrollbar-track {
	border-radius: 10px;
	background-color: transparent;
}

body::-webkit-scrollbar
{
	width: 12px;
	background-color: transparent;
}

body::-webkit-scrollbar-thumb
{
	border-radius: 10px;
	background-color: transparent;
}

button {
	cursor: pointer;
	appearance: none;
	border: none;
	outline: none;
	background: none;
}

.app {
	display: flex;

	main {
		flex: 1 1 0;
		padding: 1rem 0 1rem 1.5rem;
		display: block;
	}
}

@media screen and (max-width: 1000px) {
	.app {
		display: flex;

		main {
			flex: 1 1 0;
			padding: 2rem 2.3rem;
		}
	}
}

@media screen and (max-width: 768px) {
	.app {
		display: flex;

		main {
			flex: 1 1 0;
			padding: 2rem 1.6rem;
		}
	}
}
</style>