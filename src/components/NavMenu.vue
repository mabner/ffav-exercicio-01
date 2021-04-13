<template>
	<div class="navmenu">
		<nav>
			<ul>
				<NavMenuItems v-for="item in items" :key="item" :item="item" />
			</ul>
		</nav>
	</div>
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
