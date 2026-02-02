<script lang="ts">
	let { imgSrc, imgAlt, title, content, stack } = $props();
</script>

<div class="card">
	<img src={imgSrc} alt={imgAlt} />
	<h3>{title}</h3>
	<p>{content}</p>
	<p>{stack}</p>
</div>

<style lang="scss">
	.card {
		border-radius: 1rem;
		min-height: 30rem;
		display: flex;
		flex-direction: column;
		align-items: center;
		gap: 1rem;
		backdrop-filter: blur(0.3rem);
		border: 0.2rem solid $bg-secondary;
		color: $text-title;

		& img {
			width: 100%;
			height: 15rem;
			border-radius: 1rem 1rem 0 0;
		}
	}
</style>
