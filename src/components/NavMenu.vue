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

<style>
	.navmenu {
		background: #35495e;
		color: #fff;
	}
	.navmenu a {
		color: #fff;
	}
	.navmenu a:hover {
		color: #42b983;
	}
</style>
