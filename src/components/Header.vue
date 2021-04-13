<template>
	<header>
		<div class="header">
			<h1>{{ title }}</h1>
		</div>
	</header>
</template>

<script>
	export default {
		name: 'Header',
		props: {
			title: String,
		},
	};
</script>

<style>
	.header {
		background: #42b983;
		color: #fff;
	}
</style>
