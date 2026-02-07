<script lang="ts">
	import '$lib/scss/global.scss';
	import Nav from '$lib/components/layouts/Nav.svelte';

	let { children } = $props();
</script>

<Nav />
{@render children()}
