<script>
	import Card from '../../ui/Card.svelte';
</script>

<section id="projects" class="projects">
	<h2>Projects</h2>
	<div class="projects__card-wrapper">
		<Card
			imgSrc="/img/projects/portfolio_v1/portfolio_1.png"
			imgAlt="photo"
			title="EnzoDev v1"
			content="This is the first version of my portfolio, a space to explore my web projects and technical experiments."
			stacks={['HTML', 'SCSS', 'SVELTE']}
			githubUrl="https://github.com/Boursier-Enzo/portfolio.git"
			liveUrl="https://portfolio-boursier-enzo.netlify.app/"
			date="12/02/2026"
		/>
	</div>
</section>

<style lang="scss">
	.projects {
		width: 100%;
		min-height: 100vh;
		scroll-margin-top: 8rem;
		margin-top: 5rem;
		display: flex;
		align-items: center;
		flex-direction: column;
		gap: 3rem;
		@include md {
			margin-top: 15rem;
		}

		& h2 {
			font-size: $font-size-5xl;
			color: $text-code;

			@media screen and (max-width: (525px)) {
				font-size: $font-size-2xl;
			}
		}

		&__card-wrapper {
			width: 90%;
			height: 50%;
			display: flex;
			flex-wrap: wrap;
			gap: 3rem;
			justify-items: center;
			align-items: center;
			justify-content: center;
		}
	}
</style>
