<template>
	<li>
		<a :href="item.link">{{ item.text }}</a>
	</li>
</template>

<script>
	export default {
		name: 'NavMenuItems',
		props: {
			item: String,
		},
	};
</script>

<style scoped></style>
