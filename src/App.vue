<template>
	<div id="app">
		<div class="main">
			<Header class="header" title="FFAV - Exercício 1" />
			<NavMenu :items="menuItems" />
		</div>
	</div>
</template>

<script>
	import Header from './components/Header';
	import NavMenu from './components/NavMenu';

	export default {
		name: 'App',
		components: {
			Header,
			NavMenu,
		},
    data() {
      return {
        menuItems: [
          { text: "Core Docs", link: "https://vuejs.org"},
          { text: "Forum", link: "https://forum.vuejs.org"},
          { text: "Community", link: "https://chat.vuejs.org"},
          { text: "Twitter", link: "https://twitter.com/vuejs"},
          { text: "News", link: "https://news.vuejs.org"},
        ],
      }
    }
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
