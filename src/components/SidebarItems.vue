<template>
	<a :href="sidebar.link">{{ sidebar.text }}</a>
</template>

<script>
	export default {
		props: {
			sidebar: Object,
		},
	};
</script>

<style scoped></style>
