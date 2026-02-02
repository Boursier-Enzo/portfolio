<script>
	import Card from '$lib/components/ui/Card.svelte';
</script>

<div id="projects" class="projects">
	<h2>Projects</h2>
	<div class="projects__card-wrapper">
		<Card
			imgSrc="/img/IMG_4825.JPG"
			imgAlt="photo"
			title="Test"
			content="Ceci est un projet"
			stack="js/html/scss"
		/>
		<Card imgSrc="" imgAlt="" title="Test" content="Ceci est un projet" stack="js/html/scss" />
		<Card imgSrc="" imgAlt="" title="Test" content="Ceci est un projet" stack="js/html/scss" />
	</div>
</div>

<style lang="scss">
	.projects {
		width: 100%;
		height: 100vh;
		display: flex;
		align-items: center;
		flex-direction: column;
		gap: 5rem;

		& h2 {
			font-size: $font-size-5xl;
			color: $text-code;
		}

		&__card-wrapper {
			width: 90%;
			height: 50%;
			display: grid;
			grid-template-columns: repeat(auto-fit, minmax(25rem, 1fr));
			gap: 1rem;
		}
	}
</style>
