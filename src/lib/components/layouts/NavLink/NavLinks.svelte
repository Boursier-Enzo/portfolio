<script lang="ts">
	export let links: { name: string; active: boolean }[] = [];
	export let burgerState: boolean | undefined;
	export let handleClick: (i: number) => void;
</script>

{#each links as link, i (link.name)}
	<li>
		<a
			class={`link ${link.active}`}
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
	<button
		class="button"
		onclick={() => window.open('/img/CV Boursier Enzo AlternanceStage V5.pdf', '_blank')}
	>
		<span class="button__text">Resume</span>
		<svg class="button__icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"
			><path
				d="M416 221.25V416a48 48 0 01-48 48H144a48 48 0 01-48-48V96a48 48 0 0148-48h98.75a32 32 0 0122.62 9.37l141.26 141.26a32 32 0 019.37 22.62z"
				fill="none"
				stroke="currentColor"
				stroke-linejoin="round"
				stroke-width="32"
			/><path
				d="M256 56v120a32 32 0 0032 32h120M176 288h160M176 368h160"
				fill="none"
				stroke="currentColor"
				stroke-linecap="round"
				stroke-linejoin="round"
				stroke-width="32"
			/></svg
		>
	</button>
</li>

<style lang="scss">
	.link {
		color: $text-body;
		text-decoration: none;
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
		cursor: pointer;
		&__icon {
			width: 1rem;
			height: 1rem;
		}

		@media (hover: hover) {
			&:hover {
				box-shadow: 0 0 1rem $accent-cyan;
			}
		}
	}
</style>
