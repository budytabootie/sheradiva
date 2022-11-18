<template>
	<main :class="`${link}-page`">
        <div class="overflow">
            <div class="container">
                <div class="Brand C1">
                    <iconBrand1 />
                </div>
                <div class="Brand C2">
                    <iconBrand2 />
                </div>
                <div class="Brand C3">
                    <iconBrand3 />
                </div>
                <div class="Brand C4">
                    <iconBrand4 />
                </div>
            </div>
        </div>
    </main>
</template>

<script setup>
import iconBrand1 from '../../assets/Brand/brand1.vue'
import iconBrand2 from '../../assets/Brand/brand2.vue'
import iconBrand3 from '../../assets/Brand/brand3.vue'
import iconBrand4 from '../../assets/Brand/brand4.vue'

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
main {
    background-color: #F3F5FA;
    
    .overflow {
        display: block;
        .container {
            width: 93%;
            height: 104px;
            display: flex;
            justify-content: center;
            
            .Brand {
                width: 148px;
                height: 45px;
                justify-items: start;
                margin-top: auto;
                margin-bottom: auto;
                margin-left: calc(155px / 2);
                margin-right: calc(155px / 2);
            }
        }
        
        @media screen and (max-width: 768px) {
            .container {
                justify-content: flex-start;
                width: 20%;
                overflow: scroll;
                display: flex;
                justify-items: center;
            }
        }
    }
}
</style>