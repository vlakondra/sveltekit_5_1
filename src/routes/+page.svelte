<script>
	import Comp1 from '../lib/comp1.svelte';
	let n = $state(10);
	let arr = $state([1, 2, 3]);
</script>

<h1>Welcome to SvelteKit--{n}</h1>

<Comp1 test={n} />

<button onclick={() => n++}>BUTTON</button>

<p>
	<button onclick={() => arr.push(arr.length)}>BTN</button>
</p>
{#each arr as item}
	<p class="first">{item}</p>
{/each}

<style>
	.first {
		background-color: blueviolet;
		color: antiquewhite;
		width: 10%;
	}
</style>
