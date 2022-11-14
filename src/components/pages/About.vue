<template>
	<main :class="`${head}-page`">
		<div class="head" :id="link">
			<h1 class="hide">TENTANG KAMI</h1>
			<hr class="about hide">
		</div>
	</main>
</template>

<script setup>
import { ref, onMounted } from 'vue'
let firstOpacity = ref(0.2)
let numberH1 = ref(300)
let textH1 = ref(numberH1.value + 'px')
let numberHR = ref(200)
let textHR = ref(numberHR.value + 'px')
let mainTag = "";

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

onMounted(() =>{
	const eventScroll = document.getElementsByTagName("main")[0];
	mainTag = document.getElementById(props.link)
	let topOfSection = mainTag.offsetTop;
	let botOfSection = topOfSection + mainTag.offsetHeight;
	let userWindow = window.innerHeight;

	console.log(document.querySelector('#' + props.link + ' h1').style);
	// .forEach(item => {console.log(item)})

	eventScroll.addEventListener('wheel',(e) => {
		const rangeTopUserWindow = topOfSection - userWindow;
		const rangeBotUserWindow = topOfSection + 15;
		const currTar = Number(String(window.pageYOffset).split(".")[0])
		const rangeWidth = Number(String(topOfSection / rangeTopUserWindow + 7).split(".")[0])
		// console.log(currTar + "|" + topOfSection + "|" + rangeTopUserWindow );
		console.log(e.deltaY);
		if ( currTar > rangeTopUserWindow && e.deltaY >= 2) {
			mainTag = document.querySelector('#' + props.link + ' h1')
			const mainTag1 = document.querySelector('#' + props.link + ' hr')
			mainTag.classList.add('show')
			mainTag1.classList.add('show')
		} else if (currTar < rangeTopUserWindow + 80 && e.deltaY < -2) {
			mainTag = document.querySelector('#' + props.link + ' h1')
			const mainTag1 = document.querySelector('#' + props.link + ' hr')
			mainTag.classList.remove('show')
			mainTag1.classList.remove('show')
		}
		// else {

		// }

	// 	// console.log(window.height);

	// 	// const currTar = String(Number(window.pageYOffset) / numberTextSize.value).split(".")[0] ;

	// 	// text.value = currTar
	// 	// numberTextSize.value = currTar
	// 	// textSize.value = numberTextSize.value + 'px'
	// 	// console.log(currTar);
	})

})
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@500&display=swap');
main {
	div {
		&.head {

			width: 100%;
			height: 261px;
			display: block;
  			justify-content: center;

			h1 {
				color: #37517E;
				width: 185px;
				height: 29px;
				margin-left: auto;
				margin-right: auto;
				text-align: center;
				font-family: 'Inter', sans-serif;
				transition: 1.5s ease-out;

				&.hide {
					transform: translateX(300px);
					opacity: 0;
				}

				&.show {
					transform: translateX(0px);
					opacity: 1;
				}
			}

			hr {
				&.about {
					width: 136px;
					margin-left: auto;
					margin-right: auto;
					text-align: center;
					border: solid transparent 1px;
					border-top: solid #47B2E4 2px;
					transition: 1s ease-out;
					
				}
				&.hide {
					transform: translateX(300px);
					opacity: 0;
				}

				&.show {
					transform: translateX(0px);
					opacity: 1;
				}
			}
		}
	}
}
</style>