<template>
	<aside :class="`${is_expanded && 'is_expanded'}`">

		<div class="logo">
			<img src="../assets/Rudy_1.webp" alt="Rudy">
		</div>

		<div class="menu-toggle-wrap" id="menu-toggle-wrap">
			<button class="menu-toggle" @click="ToggleMenu">
				<span class="material-icons">keyboard_double_arrow_right</span>
			</button>
		</div>

		<h3>Menu</h3>

		<MenuVue />

	</aside>
</template>
<script setup>
import { ref, onMounted } from 'vue'

import MenuVue from './menu/Menu.vue'

const is_expanded = ref(localStorage.getItem("is_expanded") === "true")

const ToggleMenu = () => {
	is_expanded.value = !is_expanded.value

	localStorage.setItem("is_expanded", is_expanded.value)
}

</script>

<style lang="scss">
aside {
	position: fixed;
	display: flex;
	flex-direction: column;
	width: calc(2rem + 2rem);
	min-height: 100vh;
	overflow: hidden;
	padding: 1rem;
	z-index: 99;

	background-color: var(--light-alt);
	color: var(--light);

	transition: 0.4s ease-out;

	.logo {
		margin-bottom: 1rem;

		img {
			width: 2rem;
		}
	}

	.menu-toggle-wrap {
		display: flex;
		justify-content: flex-end;
		margin-bottom: 1rem;

		position: relative;
		top: 0;
		transition: 0.4s ease-out;

		.menu-toggle {
			transition: 0.4s;

			.material-icons {
				font-size: 2rem;
				color: var(--grey);
				transition: 0.4s;
			}

			&:hover {
				.material-icons {
					color: var(--primary);
					transform: translateX(0.4rem);
				}
			}
		}
	}

	h3 {
		padding-left: 2rem;
		opacity: 0;
		transition: 0.3s ease-out;
	}

	.button .text {
		opacity: 0;
		transition: 0.3s ease-out;
	}

	.menu {
		margin: 0 -1rem;

		.button {
			display: flex;
			align-items: center;
			text-decoration: none;

			padding: 0.5rem 1rem;
			transition: 0.2s ease-out;

			.collapsible {
				width: 100%;
				display: flex;
				flex-direction: row;
				justify-content: space-between;
			}

			.material-icons {
				font-size: 2rem;
				color: var(--grey);
				transition: 0.2s ease-out;
			}

			.text {
				color: var(--grey);
				transition: 0.2s ease-out;
			}

			&.router-link-exact-active {
				border-right: 5px solid var(--primary);
			}
		}
	}



	&.is_expanded {
		width: var(--sidebar-width);

		position: fixed;
		z-index: 99;


		.menu-toggle-wrap {
			top: -3rem;


			.menu-toggle {
				transform: rotate(-180deg);
			}
		}

		h3,
		.button .text {
			opacity: 1;
		}

		h3 {
			color: var(--grey);
			font-size: 0.875rem;
			margin-bottom: 0.5rem;
			text-transform: uppercase;
		}

		.button {
			.material-icons {
				margin-right: 0.3rem;
			}
		}
	}
}
</style>