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

<style scoped></style>
