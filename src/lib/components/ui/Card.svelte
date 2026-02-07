<script lang="ts">
	let { imgSrc, imgAlt, title, content, stacks, githubUrl, liveUrl } = $props();
</script>

<div class="card">
	<img src={imgSrc} alt={imgAlt} />
	<h3>{title}</h3>
	<p>{content}</p>
	<ul>
		{#each stacks as stack (stack)}
			<li>{stack}</li>
		{/each}
	</ul>
	<ul>
		<a href={githubUrl} target="_blank" rel="external noopener noreferrer">
			<svg xmlns="http://www.w3.org/2000/svg" class="ionicon" viewBox="0 0 512 512"
				><path
					d="M256 32C132.3 32 32 134.9 32 261.7c0 101.5 64.2 187.5 153.2 217.9a17.56 17.56 0 003.8.4c8.3 0 11.5-6.1 11.5-11.4 0-5.5-.2-19.9-.3-39.1a102.4 102.4 0 01-22.6 2.7c-43.1 0-52.9-33.5-52.9-33.5-10.2-26.5-24.9-33.6-24.9-33.6-19.5-13.7-.1-14.1 1.4-14.1h.1c22.5 2 34.3 23.8 34.3 23.8 11.2 19.6 26.2 25.1 39.6 25.1a63 63 0 0025.6-6c2-14.8 7.8-24.9 14.2-30.7-49.7-5.8-102-25.5-102-113.5 0-25.1 8.7-45.6 23-61.6-2.3-5.8-10-29.2 2.2-60.8a18.64 18.64 0 015-.5c8.1 0 26.4 3.1 56.6 24.1a208.21 208.21 0 01112.2 0c30.2-21 48.5-24.1 56.6-24.1a18.64 18.64 0 015 .5c12.2 31.6 4.5 55 2.2 60.8 14.3 16.1 23 36.6 23 61.6 0 88.2-52.4 107.6-102.3 113.3 8 7.1 15.2 21.1 15.2 42.5 0 30.7-.3 55.5-.3 63 0 5.4 3.1 11.5 11.4 11.5a19.35 19.35 0 004-.4C415.9 449.2 480 363.1 480 261.7 480 134.9 379.7 32 256 32z"
					fill="none"
					stroke="currentColor"
					stroke-linecap="round"
					stroke-linejoin="round"
					stroke-width="32"
				/></svg
			><span>Source</span></a
		>
		<a href={liveUrl} target="_blank" rel="external noopener noreferrer"
			><svg xmlns="http://www.w3.org/2000/svg" class="ionicon" viewBox="0 0 512 512"
				><path
					d="M255.66 112c-77.94 0-157.89 45.11-220.83 135.33a16 16 0 00-.27 17.77C82.92 340.8 161.8 400 255.66 400c92.84 0 173.34-59.38 221.79-135.25a16.14 16.14 0 000-17.47C428.89 172.28 347.8 112 255.66 112z"
					fill="none"
					stroke="currentColor"
					stroke-linecap="round"
					stroke-linejoin="round"
					stroke-width="32"
				/><circle
					cx="256"
					cy="256"
					r="80"
					fill="none"
					stroke="currentColor"
					stroke-miterlimit="10"
					stroke-width="32"
				/></svg
			><span>Live Demo</span></a
		>
	</ul>
</div>

<style lang="scss">
	.card {
		@include shadow(0deg, 1rem, 0.3rem);

		border-radius: 1.2rem;
		width: 25rem;
		height: 35rem;
		display: flex;
		flex-direction: column;
		gap: 2rem;
		background-color: #1e293b;
		color: $text-title;
		transition: all 0.5s ease;

		@media screen and (max-width: (525px)) {
			width: 20rem;
			height: 30rem;
		}

		@media (hover: hover) {
			&:hover {
				@include shadow(3deg, 1.2rem, 0.6rem);
			}
		}

		& > *:not(img) {
			margin-left: 1rem;
		}

		& img {
			width: 100%;
			height: 15rem;
			border-radius: 1.2rem 1.2rem 0 0;
			object-fit: fill;

			@media screen and (max-width: (525px)) {
				height: 10rem;
			}
		}

		& h3 {
			font-size: $font-size-xl;
			@media screen and (max-width: (525px)) {
				font-size: $font-size-lg;
			}
		}

		& p {
			width: 80%;
			height: 15%;
			color: $text-body;
			@media screen and (max-width: (525px)) {
				font-size: $font-size-sm;
			}
		}

		& ul {
			display: flex;
			gap: 1rem;
			list-style: none;

			& li {
				padding: 0.5rem;
				border-radius: 0.3rem;
				font-size: $font-size-xs;
				background-color: #1a2035;
				color: $text-code;
				border: 0.1rem solid $accent-cyan;

				@media screen and (max-width: (525px)) {
					font-size: $font-size-sm;
				}
			}

			& a {
				display: flex;
				align-items: center;
				gap: 0.5rem;
				text-decoration: none;
				& svg {
					width: 1rem;
					color: $text-body;
				}

				& span {
					font-size: $font-size-sm;
					color: $text-body;

					@media screen and (max-width: (525px)) {
						font-size: $font-size-xs;
					}
				}
			}
		}
	}
</style>
