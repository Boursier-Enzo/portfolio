<script lang="ts">
	import Nav from '$lib/components/layouts/Nav.svelte';
	import '$lib/scss/global.scss';

	let { children } = $props();
</script>

<div class="app">
	<Nav />
	{@render children()}
</div>

<style lang="scss">
	:global(html) {
		margin: 0;
		padding: 0;
		width: 100vw;
		max-width: 100vw;
		overflow-x: hidden;
	}

	:global(body) {
		margin: 0;
		padding: 0;
		width: 100vw;
		max-width: 100vw;
		overflow-x: hidden;
	}

	.app {
		width: 100vw;
		max-width: 100vw;
		min-height: 100vh;
		margin: 0;
		padding: 0;
		overflow-x: hidden;
		position: relative;
	}
</style>
