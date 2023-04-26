<script lang="ts">
	let startDate: number = 2023;
	let title = 'Mes Petits Plats';

	const addOne = () => {
		total += 1;
	};

	$: double = total * 2;

	let total = 0;
</script>

<h1 class="pl-5 my-8">{title.toUpperCase()}</h1>
<p>De mère en filles depuis {startDate}</p>

<button on:click={addOne}>Add 1</button>
<div>Total: {total} carotte{total > 1 ? '' : 's'}</div>
<div>Double: {double}</div>

<style>
</style>
