<script>
	import Card from '../../ui/Card.svelte';
</script>

<section id="projects" class="projects">
	<h2>Projects</h2>
	<div class="projects__card-wrapper">
		<Card
			imgSrc="/img/projects/portfolio_v1/portfolio_1.png"
			imgAlt="photo EnzoDev v1"
			title="EnzoDev v1"
			content="This is the first version of my portfolio, a space to explore my web projects and technical experiments."
			stacks={['HTML', 'SCSS', 'SVELTE']}
			githubUrl="https://github.com/Boursier-Enzo/portfolio.git"
			liveUrl="https://portfolio-boursier-enzo.netlify.app/"
			date="12/02/2026"
		/>
		<Card
			imgSrc="img/projects/aderm/aderm_1.png"
			imgAlt="photo ADéR.M"
			title="ADéR.M"
			content="A live website I designed, developed, and deployed on o2switch, including visual identity, project management, and team training."
			stacks={['GESTION DE PROJET' , 'WORDPRESS', 'FORMATION']}
			githubUrl=""
			liveUrl="https://association-adermaroc.org/"
			date="06/06/2025"
		/>
		<Card
			imgSrc="/img/projects/sa-hlm/sa-hml_1.png"
			imgAlt="photo SA-HLM Project"
			title="SA-HLM"
			content="A collaborative project in which I contributed to the design of the mockup and the development of the website."
			stacks={['HTML' , 'CSS', 'JS']}
			githubUrl="https://github.com/Boursier-Enzo/sa-hlm-project.git"
			liveUrl="https://sa-hlm-project.netlify.app/"
			date="15/12/2025"
		/>
		<Card
			imgSrc="/img/projects/love-bot/love-bot_1.png"
			imgAlt="photo LoveBot"
			title="LoveBot"
			content="I made a Python Discord bot that says hello and goodbye, with two actions: hug and check."
			stacks={['PYTHON']}
			githubUrl="https://github.com/Boursier-Enzo/love-bot.git"
			liveUrl=""
			date="25/03/2026"
		/>
	</div>
</section>

<style lang="scss">
	.projects {
		width: 100%;
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
