<script lang="ts">
	import { recettes } from './recettes';

	let display = false;

	function handleClick() {
		console.log('Hello');
	}
</script>

{#each recettes as recette}
	<!-- svelte-ignore a11y-click-events-have-key-events -->
	<p
		class:bg-red-500={recette.id % 2 == 0}
		class:bg-blue-700={recette.id % 2 != 0}
		on:click={() => (display = !display)}
	>
		{recette.title}
	</p>
{/each}

{#if display}
	<div>COUCOU !</div>
{/if}
