<script lang="ts">
	import Nav from '$lib/components/layouts/Nav.svelte';
	import '$lib/scss/global.scss';

	let { children } = $props();
</script>

<Nav />
{@render children()}
