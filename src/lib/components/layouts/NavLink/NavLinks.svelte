<script lang="ts">
	export let links: { name: string; active: boolean }[] = [];
	export let burgerState: boolean | undefined;
	export let handleClick: (i: number) => void;
</script>

{#each links as link, i (link.name)}
	<li>
		<a
			class={`link ${link.active && 'link--active'}`}
			onclick={() => {
				handleClick(i);
				burgerState = false;
			}}
			href={`#${link.name}`}
			>_{link.name}
		</a>
	</li>
{/each}
<li>
	<a class="button" href="#contact">
		<svg class="button__icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="#00f5ff">
			<path
				d="M23.954,5.542,15.536,13.96a5.007,5.007,0,0,1-7.072,0L.046,5.542C.032,5.7,0,5.843,0,6V18a5.006,5.006,0,0,0,5,5H19a5.006,5.006,0,0,0,5-5V6C24,5.843,23.968,5.7,23.954,5.542Z"
			/>
			<path
				d="M14.122,12.546l9.134-9.135A4.986,4.986,0,0,0,19,1H5A4.986,4.986,0,0,0,.744,3.411l9.134,9.135A3.007,3.007,0,0,0,14.122,12.546Z"
			/>
		</svg>
		<span class="button__text">Hire Me</span>
	</a>
</li>

<style lang="scss">
	.link {
		color: $text-body;
		text-decoration: none;

		&--active {
			color: $text-title;
		}
	}

	.button {
		display: flex;
		align-items: center;
		padding: 0.5rem 1rem 0.5rem 1rem;
		background-color: $bg-secondary;
		border: solid $text-code 0.1rem;
		border-radius: 0.3rem;
		text-decoration: none;
		color: $accent-cyan;
		box-shadow: 0 0 0.5rem $accent-cyan;
		transition: box-shadow 0.5s ease-in-out;
		white-space: nowrap;
		gap: 0.5rem;

		&__icon {
			width: 1rem;
			height: 1rem;
		}

		&:hover {
			box-shadow: 0 0 1rem $accent-cyan;
		}
	}
</style>
