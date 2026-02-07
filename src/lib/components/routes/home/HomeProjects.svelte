<script>
	import Card from '../../ui/Card.svelte';
</script>

<section id="projects" class="projects">
	<h2>Projects</h2>
	<div class="projects__card-wrapper">
		<Card
			imgSrc="/img/projects/portfolio_v1/portfolio_1.png"
			imgAlt="photo"
			title="DevPortfolio v1"
			content="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras pretium, libero ut imperdiet efficitur, est risus laoreet est, vitae suscipit nisi tortor ut ligula. "
			stacks={['HTML', 'SCSS', 'JS']}
			githubUrl="https://openclassrooms.com/fr/courses/1603881-creez-votre-site-web-avec-html5-et-css3/1604646-creez-un-lien-hypertexte-en-html"
			liveUrl="https://openclassrooms.com/fr/courses/1603881-creez-votre-site-web-avec-html5-et-css3/1604646-creez-un-lien-hypertexte-en-html"
		/>
		<Card
			imgSrc="/img/projects/portfolio_v1/portfolio_1.png"
			imgAlt="photo"
			title="DevPortfolio v1"
			content="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras pretium, libero ut imperdiet efficitur, est risus laoreet est, vitae suscipit nisi tortor ut ligula. "
			stacks={['HTML', 'SCSS', 'JS']}
			githubUrl="https://openclassrooms.com/fr/courses/1603881-creez-votre-site-web-avec-html5-et-css3/1604646-creez-un-lien-hypertexte-en-html"
			liveUrl="https://openclassrooms.com/fr/courses/1603881-creez-votre-site-web-avec-html5-et-css3/1604646-creez-un-lien-hypertexte-en-html"
		/>
		<Card
			imgSrc="/img/projects/portfolio_v1/portfolio_1.png"
			imgAlt="photo"
			title="DevPortfolio v1"
			content="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras pretium, libero ut imperdiet efficitur, est risus laoreet est, vitae suscipit nisi tortor ut ligula. "
			stacks={['HTML', 'SCSS', 'JS']}
			githubUrl="https://openclassrooms.com/fr/courses/1603881-creez-votre-site-web-avec-html5-et-css3/1604646-creez-un-lien-hypertexte-en-html"
			liveUrl="https://openclassrooms.com/fr/courses/1603881-creez-votre-site-web-avec-html5-et-css3/1604646-creez-un-lien-hypertexte-en-html"
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
