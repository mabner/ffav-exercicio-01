<template>
	<div class="sidebar">
		<SidebarItems v-for="item in sidebarMenu" :key="item" :sidebar="item" />
	</div>
</template>

<script>
	import SidebarItems from './SidebarItems';
	export default {
		components: {
			SidebarItems,
		},
		props: {
			sidebarMenu: Array,
		},
	};
</script>

<style>
	.sidebar a {
		display: block;
		color: #fff;
		padding: 10px;
	}
	.sidebar a:hover {
		color: #42b983;
	}
	.sidebar {
		background: #35495e;
	}
</style>
