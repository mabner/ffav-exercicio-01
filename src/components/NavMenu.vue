<template>
	<nav>
		<ul>
			<NavMenuItems
				v-for="item in items"
				:key="item"
				:item="item"
			/>
		</ul>
	</nav>
</template>

<script>
	import NavMenuItems from './NavMenuItems';
	export default {
		name: 'NavMenu',
		components: {
			NavMenuItems,
		},
		props: {
			items: Array,
		},
	};
</script>

<style scoped></style>
