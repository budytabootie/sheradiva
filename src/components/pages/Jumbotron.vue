<template>
	<main :class="`${link}-page`" :id="link">
		<div class="container">
			<div class="column">
				<div class="text">
					<h1>Solusi Terbaik Untuk Menjaga Yangmu</h1>
					<p>Perluas Jaringan Bisnis Dan Bangun Team Hebat Kamu Untuk Sukses Bersama</p>
				</div>
				<a href="">
					<div class="button">
						<span>Gabung Sekarang</span>
					</div>
				</a>
			</div>
			<div class="column svg">
				<imageOfJumbo />
			</div>
		</div>
	</main>
</template>

<script setup>
import imageOfJumbo from '../../assets/imageOfJumbo.vue'

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
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@200;400;500;700&display=swap');

main {
	font-family: 'Inter', sans-serif;
	background-color: #37517E;

	.container {
		width: 100%;
		height: 514px;
		display: flex;
		align-items: center;

		.column {
			width: 490px;
			margin: auto;
			color: #F5F5F5;
			
			.text {
				h1 {
					font-weight: 700;
					font-size: 32px;
				}

				p {
					margin-top: 17px;
					font-weight: 500;
					font-size: 15px;
				}
			}
			
			a {
				text-decoration: none;
				color: #F5F5F5;
				.button {
					margin-top: 57px;
					display: block;
					width: 122px;
					height: 34px;
					line-height: 30px;
					font-weight: 500;
					background-color: #47B2E4;
					text-align: center;
					border-radius: 20px;
					
					span {
						font-size: 10px;
						
					}
				}
			}
		}
	}
	
	@media screen and (max-width: 768px) {
		.container {
		width: calc( 100vw - 5rem );
		height: 50vh;
		background-color: #37517E;
		display: flex;
		flex-direction: column-reverse;
		align-items: center;
		
		.column {
			width: 50%;
			color: #F5F5F5;
			text-align: center;
			
			.text {
				h1 {
					font-weight: 700;
					font-size: 16px;
				}
				
				p {
					margin-top: 10px;
					font-weight: 500;
					font-size: 7px;
				}
			}
			
			a {
				text-decoration: none;
				color: #F5F5F5;
				.button {
					margin-top: 10px;
					display: block;
					width: 122px;
					height: 34px;
					margin-left: auto;
					margin-right: auto;
					
					
					span {
						font-size: 10px;
						
					}
				}
			}

			svg {
				width: 140px;
				height: 20vh;
			}
		}
	}
}
}
</style> 