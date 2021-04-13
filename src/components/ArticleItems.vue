<template>
	<section>
		<article>
			<h3>{{ article.title }}</h3>
			<p>{{ article.text }}</p>
		</article>
	</section>
</template>

<script>
	export default {
		props: {
			article: Object,
		},
	};
</script>

<style scoped></style>
