<script>
	import HomeContact from '$lib/components/routes/home/HomeContact.svelte';
	import HomeExperiences from '$lib/components/routes/home/HomeExperiences.svelte';
	import HomeHeader from '$lib/components/routes/home/HomeHeader.svelte';
	import HomeProjects from '$lib/components/routes/home/HomeProjects.svelte';
</script>

<main class="main__content">
	<HomeHeader />
	<HomeProjects />
	<HomeExperiences />
	<HomeContact />
</main>

<style lang="scss">
	.main__content {
		width: 100%;
	}
</style>
