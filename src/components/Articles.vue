<template>
	<div class="articles">
		<ArticleItems v-for="item in articles" :key="item" :article="item" />
	</div>
</template>

<script>
	import ArticleItems from './ArticleItems';

	export default {
		components: {
			ArticleItems,
		},
		props: {
			articles: Array,
		},
	};
</script>

<style scoped></style>
