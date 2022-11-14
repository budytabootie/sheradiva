<template>
	<div class="menu">
		<a>
			<MenuItem v-for="(item, index) in menuTree" :key="index" :link="item.link" :label="item.label" :icon="item.icon" :depth="0"
				:data="item.children" />
		</a>
	</div>
</template>

<script>
import MenuItem from './MenuItem.vue'

export default {
	name: "recursive-menu",
	data: () => ({
		menuTree: [
			{
				label: 'About',
				link: 'About',
				icon: 'manage_search',
			},
			{
				label: 'Product',
				link: 'Product',
				icon: 'support_agent',
				children: [
					{
						label: "Web Development",
						link: 'Web-Development',
						icon: "screen_search_desktop",
						children: [
							{
								label: 'Web Applications',
								link: 'Web-Applications',
								icon: "space_dashboard"
							},
							{
								label: 'Web Portals',
								link: 'Web-Portals',
								icon: "smart_button",
							},
						]
					},
					{
						label: "Mobile Applications",
						link: 'Mobile-Applications',
						icon: "smartphone",
					},
					{
						label: "Telegram Bot",
						link: 'Telegram-Bot',
						icon: "send",
					},

					{
						label: "Maintenance Support",
						link: 'Maintenance-Support',
						icon: "engineering",
					},
				]
			}
		]
	}),
	components: {
		MenuItem
	}
}
</script>

<style lang="scss" scoped>
a {

	&:hover,
	&.active {
		background-color: var(--light-blue);
	}

	&.active {
		border-right: 5px solid var(--primary);
	}
}
</style>