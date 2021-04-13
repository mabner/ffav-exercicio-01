<template>
	<div id="app">
		<div class="main">
			<Header class="header" title="FFAV - Exercício 1" />
			<NavMenu :items="menuItems" />
			<Articles :articles="articles" />
		</div>
	</div>
</template>

<script>
	import Header from './components/Header';
	import NavMenu from './components/NavMenu';
	import Articles from './components/Articles';

	export default {
		name: 'App',
		components: {
			Header,
			NavMenu,
			Articles,
		},
		data() {
			return {
				menuItems: [
					{ text: 'Core Docs', link: 'https://vuejs.org' },
					{ text: 'Forum', link: 'https://forum.vuejs.org' },
					{ text: 'Community', link: 'https://chat.vuejs.org' },
					{ text: 'Twitter', link: 'https://twitter.com/vuejs' },
					{ text: 'News', link: 'https://news.vuejs.org' },
				],
				articles: [
					{
						title: 'Approachable',
						text: 'Already know HTML, CSS and JavaScript? Read the guide and start building things in no time!',
					},
					{
						title: 'Versatile',
						text: 'An incrementally adoptable ecosystem that scales between a library and a full-featured framework.',
					},
					{
						title: 'Performant',
						text: '20KB min+gzip Runtime. Blazing Fast Virtual DOM. Minimal Optimization Efforts',
					},
				],
			};
		},
	};
</script>

<style>
	#app {
		font-family: Avenir, Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		text-align: center;
		color: #2c3e50;
		margin-top: 60px;
	}
</style>
