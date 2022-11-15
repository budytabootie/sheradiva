<template>

	<div class="toggleService" id="toggleService">
		<a class="button" :href="`#${link}`" :id="`${link}1`">

			<span v-if="icon" class="material-icons">{{ icon }}</span>
			<span v-if="showLabel" class="text">{{ label }}</span>

			<div v-if="data" class="collapsible" @click="toggleMenu()" :style="{ paddingLeft: depth * 5 + 5 + 'px' }">
				<div class="to_right"></div>
				<div class="for_icon">

					<i class="expand material-icons" :class="{ opened: expanded }">expand_more</i>
				</div>
			</div>
		</a>
	</div>

	<div v-show="showChildren" class="items-container" :class="{ cExpanded: is_expanded }"
		:style="{ height: containerHeight }" ref="container">
		<menu-item v-for="(item, index) in data" :key="index" :data="item.children" :label="item.label"
			:icon="item.icon" :depth="depth + 1" :link="item.link" />
	</div>

</template>

<script setup>

	import { ref, onMounted, nextTick } from 'vue'

	let showChildren = ref(false);
	let expanded = ref(false);
	let containerHeight = ref(0);
	let container = ref(null);
	let overflow = ref('auto');
	let is_expanded = ref(localStorage.getItem("is_expanded") === "true");
	let menuItems = "";
	let cExpanded = props.depth * 15 + 15 + 'px';
	let beArray = "About,Product,Web-Development,Web-Applications,Web-Portals,Mobile-Applications,Telegram-Bot,Maintenance-Support"

	const props = defineProps({
		data: {
			type: Array,
		},
		label: {
			type: String,
		},
		link: {
			type: String,
		},
		icon: {
			type: String,
		},
		depth: {
			type: Number,
		},
		smallMenu: {
			type: Boolean,
		}
	})

	onMounted(() => {

		rmvClassActive()

		document.getElementById("menu-toggle-wrap").addEventListener("click", materialClick);

		menuItems = document.querySelectorAll('.toggleService a[href^="#"]');
		menuItems.forEach(item => {
			item.addEventListener('click', scrollToIdOnClick);
		});

		let bodyS = document.getElementsByTagName("main")[0];
		
		bodyS.addEventListener('touchmove', getScrollPosition, true);
		bodyS.addEventListener('wheel', getScrollPosition, true);
		bodyS.onscroll = getScrollPosition;


	})

	function rmvClassActive () {

		menuItems = Array(props.link)

		menuItems.forEach(itemS => {

			document.getElementById(itemS + `1`).addEventListener('click',(event) => {

				beArray.split(",").forEach(item => {
					document.getElementById(item + `1`).classList.remove(item)
					document.getElementById(item + `1`).classList.remove('active')
				})

				let currTar = event.currentTarget.getAttribute('href').split("#")[1]
				

				if (itemS == currTar ) {
				
				document.getElementById(itemS + `1`).classList.remove('active')
				document.getElementById(itemS + `1`).classList.add('active')

				}

			})

			

			document.getElementById(itemS + `1`).addEventListener('mouseover',(event) => {

				beArray.split(",").forEach(item => {
					if (item + `1` != event.currentTarget.getAttribute('id')) {
					document.getElementById(item + `1`).classList.add('hide')
					}
				})

				const currTar = event.currentTarget.getAttribute('href').split("#")[1]

				if (itemS == currTar ) {

				document.getElementById(itemS + `1`).classList.add(itemS)

				}

			})

			document.getElementById(itemS + `1`).addEventListener('mouseleave',(event) => {

				beArray.split(",").forEach(item => {
					document.getElementById(item + `1`).classList.remove('hide')
				})

				const currTar = event.currentTarget.getAttribute('href').split("#")[1]

				if (itemS == currTar ) {

				document.getElementById(itemS + `1`).classList.remove(itemS)

				}

			})	

		})

	}
	
	function materialClick () {
		is_expanded.value = !is_expanded.value
	}

	function showLabel() {
		return props.smallMenu ? props.depth > 0 : true;
	}

	function toggleMenu() {
		expanded.value = !expanded.value;
		if (!showChildren.value) {
			showChildren.value = true;
			nextTick(() => {
				containerHeight.value = container.value.scrollHeight + "px";
				setTimeout(() => {
					containerHeight.value = "fit-content";
					if (navigator.userAgent.indexOf("Firefox") != -1)
						containerHeight.value = "-moz-max-content"
					overflow.value = "visible";
				}, 300);
			});
			
		} else {
			containerHeight.value = container.value.scrollHeight + "px";
			overflow.value = "hidden";
			setTimeout(() => {
				containerHeight.value = 0 + "px";
			}, 10);
			setTimeout(() => {
				showChildren.value = false;
			}, 300);
		}
	}

	function getScrollPosition(){

		menuItems = Array(props.link);
		beArray.split(",").forEach(item => {
			document.getElementById(item + `1`).classList.remove(item)
		})
		menuItems.forEach(item => {

			const topHref = Number(document.getElementById(item).offsetTop) - 80;
			const botHref = topHref + Number(document.getElementById('theSection').offsetHeight);
			const currentPos = window.pageYOffset

			if (currentPos > topHref && currentPos < botHref ) {
				document.getElementById(item + '1').classList.add('active')
			} else {
				document.getElementById(item + '1').classList.remove('active')
			}


		});
		
    }

</script>



<style lang="scss" scoped>
.toggleService {
	padding: 0px 5px;
	a {
		&.About,
		&.Product,
		&.Web-Development,
		&.Web-Applications,
		&.Web-Portals,
		&.Mobile-Applications,
		&.Telegram-Bot,
		&.Maintenance-Support,
		&:hover,
		&.active {
			background-color: var(--light-blue);
			border-radius: 20px;
		}
	}

	.button {
		display: flex;
		align-items: center;
		text-decoration: none;

		padding: 1rem 0.7rem;
		transition: 0.2s ease-out;

		.material-icons {
			font-size: 2rem;
			color: var(--grey);
			transition: 0.2s ease-out;
		}
	}
}

.is_expanded {

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

	.toggleService {

		flex-direction: row;
		justify-content: space-between;
		padding: 0rem 1rem;

		.button {
			display: flex;
			align-items: center;
			text-decoration: none;
			transition: 0.1s ease-out;
			padding: 0.3rem 0.5rem 0.3rem 1.3rem;
			margin: 1rem 0rem;

			.collapsible {
				width: 100%;
				display: flex;
				flex-direction: row;
				justify-content: space-between;
				padding: 0rem 0rem;

				div {
					i {
						padding: 0rem 1rem;
						transition: all 0.3s ease;

						&.expand {


							&.opened {
								transform: rotate(180deg);
							}

						}


					}
				}

			}

			.material-icons {
				font-size: 2rem;
				color: var(--grey);
				transition: 0.2s ease-out;
			}

			.text {
				color: var(--grey);
				transition: 0.2s ease-out;
				padding: 0rem 1rem;
			}

			&.About,
			&.Product,
			&.Web-Development,
			&.Web-Applications,
			&.Web-Portals,
			&.Mobile-Applications,
			&.Telegram-Bot,
			&.Maintenance-Support,
			&:hover,
			&.active {
				background: #C2C1FB;
				border-radius: 20px;

				&.hide {
					background-color: #F3F5FA;
				}
			}
		}

		&.small-item {
			width: fit-content;
		}
	}

	.items-container {
		width: 100%;
		transition: height 0.3s ease;

		&.cExpanded {
			padding-left: v-bind(cExpanded);
		}
	}
}
</style>
<script>
	function getScrollTopByHref(element) {
		const id = element.getAttribute('href');
		return document.querySelector(id).offsetTop;
	}
	function scrollToPosition(to) {
		// Caso queira o nativo apenas
		// window.scroll({
		// top: to,
		// behavior: "smooth",
		// })
		smoothScrollTo(0, to, 2000);
	}
	function scrollToIdOnClick(event) {

		event.preventDefault();
		const to = getScrollTopByHref(event.currentTarget) - 80;
		scrollToPosition(to);

	}
	function smoothScrollTo(endX, endY, duration) {
		const startX = window.scrollX || window.pageXOffset;
		const startY = window.scrollY || window.pageYOffset;
		const distanceX = endX - startX;
		const distanceY = endY - startY;
		const startTime = new Date().getTime();

		duration = typeof duration !== 'undefined' ? duration : 400;

		// Easing function
		const easeInOutQuart = (time, from, distance, duration) => {
			if ((time /= duration / 2) < 1) return distance / 2 * time * time * time * time + from;
			return -distance / 2 * ((time -= 2) * time * time * time - 2) + from;
		};

		const timer = setInterval(() => {
			const time = new Date().getTime() - startTime;
			const newX = easeInOutQuart(time, startX, distanceX, duration);
			const newY = easeInOutQuart(time, startY, distanceY, duration);
			if (time >= duration) {
				clearInterval(timer);
			}
			window.scroll(newX, newY);
		}, 1000 / 120); // 60 fps
	};
</script>