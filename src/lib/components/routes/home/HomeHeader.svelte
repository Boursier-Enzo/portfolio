<script>
	import HomeHeaderLeftSide from './HomeHeader/HomeHeaderLeftSide.svelte';
	import HomeHeaderRightSide from './HomeHeader/HomeHeaderRightSide.svelte';
</script>

<header class="hero">
	<HomeHeaderLeftSide />
	<HomeHeaderRightSide />
</header>

<style lang="scss">
	.hero {
		width: 100%;
		height: 100vh;
		display: flex;

		@include md {
			align-items: center;
			flex-direction: column;
		}
	}
</style>
